---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 13
api_specs:
- filename: ausca-com-agent-inboxes-api-openapi.yml
  format: yaml
  label: Ausca Agent Inboxes API
  slug: ausca-com-agent-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-agent-inboxes-api-openapi.yml
- filename: ausca-com-analyze-document-api-openapi.yml
  format: yaml
  label: Ausca Analyze Document API
  slug: ausca-com-analyze-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-analyze-document-api-openapi.yml
- filename: ausca-com-artifacts-api-openapi.yml
  format: yaml
  label: Ausca Artifacts API
  slug: ausca-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-artifacts-api-openapi.yml
- filename: ausca-com-browser-sessions-api-openapi.yml
  format: yaml
  label: Ausca Browser Sessions API
  slug: ausca-com-browser-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-browser-sessions-api-openapi.yml
- filename: ausca-com-extend-inbox-api-openapi.yml
  format: yaml
  label: Ausca Extend Inbox API
  slug: ausca-com-extend-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-extend-inbox-api-openapi.yml
- filename: ausca-com-extract-text-api-openapi.yml
  format: yaml
  label: Ausca Extract Text API
  slug: ausca-com-extract-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-extract-text-api-openapi.yml
- filename: ausca-com-invocations-api-openapi.yml
  format: yaml
  label: Ausca Invocations API
  slug: ausca-com-invocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-invocations-api-openapi.yml
- filename: ausca-com-lease-browser-api-openapi.yml
  format: yaml
  label: Ausca Lease Browser API
  slug: ausca-com-lease-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-lease-browser-api-openapi.yml
- filename: ausca-com-offers-api-openapi.yml
  format: yaml
  label: Ausca Offers API
  slug: ausca-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-offers-api-openapi.yml
- filename: ausca-com-open-inbox-api-openapi.yml
  format: yaml
  label: Ausca Open Inbox API
  slug: ausca-com-open-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-open-inbox-api-openapi.yml
- filename: ausca-com-transcribe-media-api-openapi.yml
  format: yaml
  label: Ausca Transcribe Media API
  slug: ausca-com-transcribe-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-transcribe-media-api-openapi.yml
consequence_counts:
  read: 13
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ausca Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Ausca exposes 27 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ausca
provider_slug: ausca-com
slug: ausca-com-agentic-access
source_filename: ausca-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/ausca-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 14\n    connected: 13\n  by_consequence:\n    write: 14\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/agent-inboxes/{inbox_id}\n  method: delete\n  operationId: DeleteAgentInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-inboxes/{inbox_id}\n  method: get\n  operationId: GetAgentInbox\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-inboxes/{inbox_id}/messages\n  method: get\n  operationId: ListAgentInboxMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-inboxes/{inbox_id}/messages/{message_id}\n  method: get\n  operationId: GetAgentInboxMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-inboxes/{inbox_id}/messages/{message_id}/attachments/{attachment_id}/access\n  method: post\n  operationId: CreateAgentInboxAttachmentAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyze-document\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyze-document\n  method: post\n  operationId: AnalyzeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts\n  method: post\n  operationId: CommitArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/{artifact_uri}/access\n \
  \ method: post\n  operationId: CreateArtifactAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/browser-sessions/{session_id}\n  method: delete\n  operationId: CloseBrowserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/browser-sessions/{session_id}\n  method: get\n  operationId: GetBrowserSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/browser-sessions/{session_id}/connections\n  method:\
  \ post\n  operationId: ConnectBrowserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extend-inbox\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extend-inbox\n  method: post\n  operationId: ExtendInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract-text\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/extract-text\n  method: post\n  operationId: ExtractText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invocations/prepare\n  method: post\n  operationId: PrepareInvocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invocations/{invocation_id}\n  method: get\n  operationId: GetInvocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invocations/{invocation_id}/cancel\n\
  \  method: post\n  operationId: CancelInvocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lease-browser\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lease-browser\n  method: post\n  operationId: LeaseBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers\n  method: get\n  operationId: SearchOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/{offer_id}\n  method: get\n  operationId: GetOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-inbox\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-inbox\n  method: post\n  operationId: OpenInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcribe-media\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/transcribe-media\n  method: post\n  operationId: TranscribeMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ausca-com/agentic-access/ausca-com-agentic-access.yml
summary_line: 27 operations · 14 acting
tags:
- Pay-per-call APIs
- Agent Infrastructure
- Document OCR
- Media transcription
- Inbox verification
---
