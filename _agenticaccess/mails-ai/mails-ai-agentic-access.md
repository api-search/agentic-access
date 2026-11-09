---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 36
api_specs:
- filename: mails-ai-account-api-openapi.yml
  format: yaml
  label: mails-ai Account API
  slug: mails-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-account-api-openapi.yml
- filename: mails-ai-agents-api-openapi.yml
  format: yaml
  label: mails-ai Agents API
  slug: mails-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-agents-api-openapi.yml
- filename: mails-ai-api-keys-api-openapi.yml
  format: yaml
  label: mails-ai API Keys API
  slug: mails-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-api-keys-api-openapi.yml
- filename: mails-ai-billing-api-openapi.yml
  format: yaml
  label: mails-ai Billing API
  slug: mails-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-billing-api-openapi.yml
- filename: mails-ai-connected-apps-api-openapi.yml
  format: yaml
  label: mails-ai Connected Apps API
  slug: mails-ai-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-connected-apps-api-openapi.yml
- filename: mails-ai-domains-api-openapi.yml
  format: yaml
  label: mails-ai Domains API
  slug: mails-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-domains-api-openapi.yml
- filename: mails-ai-drafts-api-openapi.yml
  format: yaml
  label: mails-ai Drafts API
  slug: mails-ai-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-drafts-api-openapi.yml
- filename: mails-ai-events-api-openapi.yml
  format: yaml
  label: mails-ai Events API
  slug: mails-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-events-api-openapi.yml
- filename: mails-ai-inbound-api-openapi.yml
  format: yaml
  label: mails-ai Inbound API
  slug: mails-ai-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-inbound-api-openapi.yml
- filename: mails-ai-labels-api-openapi.yml
  format: yaml
  label: mails-ai Labels API
  slug: mails-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-labels-api-openapi.yml
- filename: mails-ai-logs-api-openapi.yml
  format: yaml
  label: mails-ai Logs API
  slug: mails-ai-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-logs-api-openapi.yml
- filename: mails-ai-messages-api-openapi.yml
  format: yaml
  label: mails-ai Messages API
  slug: mails-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-messages-api-openapi.yml
- filename: mails-ai-metrics-api-openapi.yml
  format: yaml
  label: mails-ai Metrics API
  slug: mails-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-metrics-api-openapi.yml
- filename: mails-ai-public-api-openapi.yml
  format: yaml
  label: mails-ai Public API
  slug: mails-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-public-api-openapi.yml
- filename: mails-ai-reputation-api-openapi.yml
  format: yaml
  label: mails-ai Reputation API
  slug: mails-ai-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-reputation-api-openapi.yml
- filename: mails-ai-search-api-openapi.yml
  format: yaml
  label: mails-ai Search API
  slug: mails-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-search-api-openapi.yml
- filename: mails-ai-suppression-api-openapi.yml
  format: yaml
  label: mails-ai Suppression API
  slug: mails-ai-suppression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-suppression-api-openapi.yml
- filename: mails-ai-threads-api-openapi.yml
  format: yaml
  label: mails-ai Threads API
  slug: mails-ai-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-threads-api-openapi.yml
- filename: mails-ai-webhooks-api-openapi.yml
  format: yaml
  label: mails-ai Webhooks API
  slug: mails-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 36
  safety-critical: 3
  write: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Mails Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/api-keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/oauth/grants/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/suppression/allow/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/portal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/drafts/{id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/test
operation_count: 74
overview: 'mails-ai exposes 74 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 29 write, 6 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: mails-ai
provider_slug: mails-ai
slug: mails-ai-agentic-access
source_filename: mails-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/api_mails_ai_v1.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 74\n  by_action_class:\n    acting: 38\n    connected: 36\n  by_consequence:\n    physical: 6\n    read: 36\n    write: 29\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method:\
  \ get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/batch\n  method: post\n  operationId: batchSendMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/appeal\n  method: post\n  operationId: appealMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}\n  method: get\n  operationId:\
  \ getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/{id}\n  method: patch\n  operationId: rescheduleMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/reply\n  method: post\n  operationId: replyMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/forward\n  method: post\n  operationId: forwardMessage\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/cancel\n  method: post\n  operationId: cancelMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/raw\n  method: get\n  operationId: getMessageRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/received\n  method: get\n  operationId: listReceivedMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/messages/received/wait\n  method: get\n  operationId: waitForReceivedMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/received/{id}\n  method: get\n  operationId: getReceivedMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/received/{id}/attachments\n  method: get\n  operationId: listReceivedAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/received/{id}/attachments/{attachment_id}\n  method: get\n  operationId: downloadReceivedAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/test/inbound\n  method: post\n  operationId: simulateInbound\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{id}\n  method: delete\n  operationId: archiveAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{id}/forwarding/verify\n  method: post\n  operationId: verifyAgentForwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{id}/inbox\n  method: get\n  operationId: getAgentInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys/{id}\n\
  \  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/oauth/grants\n  method: get\n  operationId: listConnectedApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oauth/grants/{id}\n  method: delete\n  operationId: revokeConnectedApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/me\n  method:\
  \ get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drafts\n  method: post\n  operationId: createDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drafts\n  method: get\n  operationId: listDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drafts/{id}\n  method: get\n  operationId: getDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drafts/{id}\n  method: patch\n  operationId: updateDraft\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drafts/{id}\n  method: delete\n  operationId: deleteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drafts/{id}/send\n  method: post\n  operationId: sendDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/threads\n  method: get\n  operationId: listThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/threads/{id}\n  method: get\n  operationId: getThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/threads/{id}\n  method: patch\n  operationId: updateThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/threads/{id}\n  method: delete\n  operationId: deleteThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/labels\n  method: get\n  operationId: listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/labels\n  method: post\n  operationId: createLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/labels/{id}\n  method: get\n  operationId: getLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/labels/{id}\n  method: patch\n  operationId: updateLabel\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/labels/{id}\n  method: delete\n  operationId: deleteLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search\n  method: get\n  operationId: searchMail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{id}/redeliver\n  method: post\n  operationId: redeliverEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events/stream\n  method: get\n  operationId: streamEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/logs\n  method: get\n  operationId: listLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method:\
  \ patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/rotate-secret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v1/webhooks/{id}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-deliveries/{id}/replay\n  method: post\n  operationId: replayWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suppression\n  method: get\n  operationId: listSuppression\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suppression/allow\n  method: post\n  operationId: allowSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suppression/allow/{id}\n  method: delete\n  operationId: revokeSuppressionAllow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/domains\n  method: post\n  operationId: createDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/verify\n  method: post\n  operationId: verifyDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reputation\n  method: get\n  operationId: getReputation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/usage\n  method: get\n  operationId: getBillingUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/billing/portal\n  method: post\n  operationId: openBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/unsubscribe\n  method: get\n  operationId: unsubscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/unsubscribe\n  method: post\n  operationId: unsubscribeOneClick\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method:\
  \ get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/mails-ai/agentic-access/mails-ai-agentic-access.yml
summary_line: 74 operations · 38 acting · 3 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Email
- Infrastructure
- Agents
---
