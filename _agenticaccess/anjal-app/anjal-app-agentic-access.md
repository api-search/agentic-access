---
acting_count: 61
action_class_counts:
  acting: 61
  connected: 51
api_specs:
- filename: anjal-app-addresses-api-openapi.yml
  format: yaml
  label: Anjal Addresses API
  slug: anjal-app-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-addresses-api-openapi.yml
- filename: anjal-app-cadences-api-openapi.yml
  format: yaml
  label: Anjal Cadences API
  slug: anjal-app-cadences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-cadences-api-openapi.yml
- filename: anjal-app-domains-api-openapi.yml
  format: yaml
  label: Anjal Domains API
  slug: anjal-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-domains-api-openapi.yml
- filename: anjal-app-drafts-api-openapi.yml
  format: yaml
  label: Anjal Drafts API
  slug: anjal-app-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-drafts-api-openapi.yml
- filename: anjal-app-inboxes-api-openapi.yml
  format: yaml
  label: Anjal Inboxes API
  slug: anjal-app-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-inboxes-api-openapi.yml
- filename: anjal-app-linkedin-outreach-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Outreach API
  slug: anjal-app-linkedin-outreach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-outreach-api-openapi.yml
- filename: anjal-app-linkedin-posts-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Posts API
  slug: anjal-app-linkedin-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-posts-api-openapi.yml
- filename: anjal-app-linkedin-searches-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Searches API
  slug: anjal-app-linkedin-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-searches-api-openapi.yml
- filename: anjal-app-linkedin-sessions-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Sessions API
  slug: anjal-app-linkedin-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-sessions-api-openapi.yml
- filename: anjal-app-linkedin-signals-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Signals API
  slug: anjal-app-linkedin-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-signals-api-openapi.yml
- filename: anjal-app-lists-api-openapi.yml
  format: yaml
  label: Anjal Lists API
  slug: anjal-app-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-lists-api-openapi.yml
- filename: anjal-app-messages-api-openapi.yml
  format: yaml
  label: Anjal Messages API
  slug: anjal-app-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-messages-api-openapi.yml
- filename: anjal-app-metrics-api-openapi.yml
  format: yaml
  label: Anjal Metrics API
  slug: anjal-app-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-metrics-api-openapi.yml
- filename: anjal-app-tenants-api-openapi.yml
  format: yaml
  label: Anjal Tenants API
  slug: anjal-app-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-tenants-api-openapi.yml
- filename: anjal-app-webhooks-api-openapi.yml
  format: yaml
  label: Anjal Webhooks API
  slug: anjal-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-webhooks-api-openapi.yml
- filename: anjal-app-websocket-api-openapi.yml
  format: yaml
  label: Anjal WebSocket API
  slug: anjal-app-websocket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-websocket-api-openapi.yml
- filename: anjal-app-workspaces-api-openapi.yml
  format: yaml
  label: Anjal Workspaces API
  slug: anjal-app-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-workspaces-api-openapi.yml
consequence_counts:
  physical: 5
  read: 51
  safety-critical: 2
  write: 54
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Anjal App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /linkedin/sessions/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{id}/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /linkedin/connections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /linkedin/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /linkedin/signals/{id}/test-webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/drafts/{did}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/send
operation_count: 112
overview: 'Anjal exposes 112 API operations that an AI agent could call, of which 61 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 51 read, 54 write, 5 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anjal
provider_slug: anjal-app
slug: anjal-app-agentic-access
source_filename: anjal-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anjal-app-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 112\n  by_action_class:\n    acting: 61\n    connected: 51\n  by_consequence:\n    write: 54\n    read: 51\n    safety-critical: 2\n    physical: 5\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{id}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{id}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{id}/keys\n  method: post\n  operationId: createWorkspaceKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{id}/keys\n  method: get\n  operationId: listWorkspaceKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{id}/keys/{key_id}\n  method: delete\n  operationId: revokeWorkspaceKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/inboxes\n  method: post\n  operationId: createInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/inboxes\n  method: get\n  operationId: listInboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}\n  method: get\n  operationId: getInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}\n  method: patch\n  operationId: updateInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}\n  method: delete\n  operationId: deleteInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/addresses\n  method: post\n  operationId: addInboxAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/addresses/{address}\n  method: delete\n  operationId: removeInboxAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/reply/{messageId}\n  method: post\n  operationId: replyMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/reply-all/{messageId}\n  method: post\n  operationId: replyAllMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/forward/{messageId}\n  method: post\n  operationId: forwardMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/threads\n  method: get\n  operationId: listThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/threads/{threadId}\n  method: get\n  operationId: getThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/threads/{threadId}\n  method: patch\n  operationId: updateThread\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/threads/{threadId}\n  method: delete\n  operationId: deleteThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: get\n  operationId: listAllMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/labels\n  method: get\n  operationId: listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v1/messages/search\n  method: get\n  operationId: searchMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages/{messageId}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages/{messageId}\n  method: patch\n  operationId: updateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/messages/{messageId}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/messages/{messageId}/raw\n  method: get\n  operationId: getMessageRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages/{messageId}/attachments\n  method: get\n  operationId: listAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages/{messageId}/attachments/{aid}\n\
  \  method: get\n  operationId: getAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages/{messageId}/attachments/{aid}/download-url\n  method: post\n  operationId: createAttachmentDownloadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /downloads/{downloadId}\n  method: get\n  operationId: getAttachmentByDownloadLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/attachment-uploads\n  method: post\n  operationId: createAttachmentUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads/{uploadId}\n  method: put\n  operationId: uploadAttachmentFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts\n  method: post\n  operationId: createDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts\n  method: get\n  operationId: listDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/inboxes/{id}/drafts/{did}\n  method: get\n  operationId: getDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/drafts/{did}\n  method: patch\n  operationId: updateDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts/{did}\n  method: delete\n  operationId: deleteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts/{did}/send\n\
  \  method: post\n  operationId: sendDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/lists\n  method: get\n  operationId: listLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/lists/{lid}\n  method: get\n\
  \  operationId: getList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/lists/{lid}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/lists/{lid}/entries\n  method: post\n  operationId: addListEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/lists/{lid}/entries/{eid}\n  method: delete\n  operationId: removeListEntry\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains\n  method: post\n  operationId: createDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/verify\n  method: get\n  operationId: verifyDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/zone-file\n  method: get\n  operationId: getDomainZoneFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n\
  \  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ws\n  method: get\n  operationId: openWebSocket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify-email\n  method: post\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenants\n  method: post\n  operationId: createTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenants\n  method: get\n  operationId: listTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenants/{id}\n  method: delete\n  operationId: deleteTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /linkedin/sessions\n  method: post\n  operationId: linkedinLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/sessions\n  method: get\n  operationId: linkedinListSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/sessions/verify\n  method: post\n  operationId: linkedinVerifyPin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/sessions/poll\n  method: post\n  operationId: linkedinPollMobileApproval\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/sessions/import\n  method: post\n  operationId: linkedinImportSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/sessions/{id}\n  method: get\n  operationId: linkedinGetSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/sessions/{id}\n  method: delete\n  operationId: linkedinRevokeSession\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /linkedin/profiles/lookup\n  method: post\n  operationId: linkedinLookupProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/connections\n  method: post\n  operationId: linkedinSendConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/connections\n  method: get\n  operationId: linkedinListConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/invitations/sent\n  method: get\n  operationId: linkedinListSentInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/messages\n  method: post\n  operationId: linkedinSendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/conversations\n  method: get\n  operationId:\
  \ linkedinListConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/conversations/{conversationUrn}/messages\n  method: get\n  operationId: linkedinListConversationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/search/content\n  method: post\n  operationId: linkedinSearchContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/posts\n  method: post\n  operationId: linkedinCreatePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/posts/by-author\n  method: get\n  operationId: linkedinListPostsByAuthor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/posts/{postUrn}/comments\n  method: get\n  operationId: linkedinListPostComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/posts/{postUrn}/reactions\n  method: get\n  operationId: linkedinListPostReactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/sessions/utilization\n  method: get\n  operationId: linkedinSessionUtilization\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/signals\n  method: get\n  operationId: linkedinListSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/signals\n  method: post\n  operationId: linkedinCreateSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/signals/{id}\n  method: get\n  operationId: linkedinGetSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/signals/{id}\n  method: patch\n  operationId: linkedinUpdateSignal\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/signals/{id}\n  method: delete\n  operationId: linkedinDeleteSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/signals/{id}/run\n  method: post\n  operationId: linkedinRunSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /linkedin/signals/{id}/matches\n  method: get\n  operationId: linkedinSignalMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/signals/{id}/deliveries\n  method: get\n  operationId: linkedinSignalDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/signals/{id}/test-webhook\n  method: post\n  operationId: linkedinSignalTestWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/signals/{id}/watchlist\n  method: get\n  operationId: linkedinSignalWatchlistList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/signals/{id}/watchlist\n  method: post\n  operationId: linkedinSignalWatchlistAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/signals/{id}/watchlist/{entryId}\n  method: delete\n  operationId: linkedinSignalWatchlistRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/searches\n  method: get\n  operationId: linkedinListSearches\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/searches\n  method: post\n  operationId: linkedinRunSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linkedin/searches/{id}\n  method: get\n  operationId: linkedinGetSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cadences\n  method: post\n  operationId: createCadence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cadences\n  method: get\n  operationId: listCadences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cadences/{id}\n  method: get\n  operationId: getCadence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cadences/{id}\n  method: patch\n  operationId: updateCadence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cadences/{id}\n  method: delete\n  operationId: deleteCadence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cadences/{id}/steps\n  method: patch\n  operationId: replaceCadenceSteps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cadences/{id}/enrollments\n  method: post\n  operationId: enrollLeadInCadence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cadences/{id}/enrollments\n  method: get\n  operationId: listCadenceEnrollments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cadences/{id}/enrollments/bulk-relink\n  method: post\n  operationId: bulkRelinkEnrollments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cadences/{id}/run-now\n  method: post\n  operationId: forceCadenceTick\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrollments/{id}\n  method: get\n  operationId: getEnrollment\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (32 KB total) ---\n# Full source: https://artifacts.apis.io/anjal-app/agentic-access/anjal-app-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/anjal-app/agentic-access/anjal-app-agentic-access.yml
summary_line: 112 operations · 61 acting · 2 human-in-the-loop
tags:
- Email
- Artificial Intelligence
- Agents
- Software-as-a-Service
- Email API
---
