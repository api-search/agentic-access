---
acting_count: 186
action_class_counts:
  acting: 186
  connected: 84
api_specs:
- filename: communicate-so-account-credentials-api-openapi.yml
  format: yaml
  label: communicate-so Account credentials API
  slug: communicate-so-account-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-account-credentials-api-openapi.yml
- filename: communicate-so-account-preferences-api-openapi.yml
  format: yaml
  label: communicate-so Account preferences API
  slug: communicate-so-account-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-account-preferences-api-openapi.yml
- filename: communicate-so-agents-api-openapi.yml
  format: yaml
  label: communicate-so Agents API
  slug: communicate-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-agents-api-openapi.yml
- filename: communicate-so-authentication-api-openapi.yml
  format: yaml
  label: communicate-so Authentication API
  slug: communicate-so-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-authentication-api-openapi.yml
- filename: communicate-so-chat-api-openapi.yml
  format: yaml
  label: communicate-so Chat API
  slug: communicate-so-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-chat-api-openapi.yml
- filename: communicate-so-discovery-api-openapi.yml
  format: yaml
  label: communicate-so Discovery API
  slug: communicate-so-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-discovery-api-openapi.yml
- filename: communicate-so-grill-api-openapi.yml
  format: yaml
  label: communicate-so Grill API
  slug: communicate-so-grill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-grill-api-openapi.yml
- filename: communicate-so-inbox-api-openapi.yml
  format: yaml
  label: communicate-so Inbox API
  slug: communicate-so-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-inbox-api-openapi.yml
- filename: communicate-so-learnings-api-openapi.yml
  format: yaml
  label: communicate-so Learnings API
  slug: communicate-so-learnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-learnings-api-openapi.yml
- filename: communicate-so-notifications-api-openapi.yml
  format: yaml
  label: communicate-so Notifications API
  slug: communicate-so-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-notifications-api-openapi.yml
- filename: communicate-so-sources-api-openapi.yml
  format: yaml
  label: communicate-so Sources API
  slug: communicate-so-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-sources-api-openapi.yml
- filename: communicate-so-teams-api-openapi.yml
  format: yaml
  label: communicate-so Teams API
  slug: communicate-so-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-teams-api-openapi.yml
- filename: communicate-so-workspace-members-api-openapi.yml
  format: yaml
  label: communicate-so Workspace members API
  slug: communicate-so-workspace-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-workspace-members-api-openapi.yml
- filename: communicate-so-workspaces-api-openapi.yml
  format: yaml
  label: communicate-so Workspaces API
  slug: communicate-so-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-workspaces-api-openapi.yml
consequence_counts:
  physical: 26
  read: 84
  safety-critical: 10
  write: 150
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Communicate So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account-credentials/{credentialId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{destinationWorkspaceId}/linked-agents/{grantId}/sources/{sourceId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{requestingWorkspaceId}/agents/{agentId}/analytics/topics/merge
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{requestingWorkspaceId}/agents/{agentId}/analytics/topics/{canonicalTopicId}/archive
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{requestingWorkspaceId}/agents/{agentId}/analytics/topics/{canonicalTopicId}/rename
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/grants/{grantId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /workspaces/{workspaceId}/agents/{agentId}/sources/{sourceId}/refresh
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/support/widget-identity/rotate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspaceId}/api-keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspaceId}/api-keys/{keyId}/permanent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agents/{agentId}/chat
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{transferId}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{transferId}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/copilot
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/messages/{messageId}/undo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/chat
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/grants/{grantId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/grill/rounds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/grill/rounds/{roundId}/questions/{questionId}/draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/grill/rounds/{roundId}/questions/{questionId}/regenerate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/grill/rounds/{roundId}/questions/{questionId}/skip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/support/rules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workspaces/{workspaceId}/agents/{agentId}/support/rules/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/agents/{agentId}/transfer
operation_count: 270
overview: 'communicate-so exposes 270 API operations that an AI agent could call, of which 186 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 84 read, 150 write, 26 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: communicate-so
provider_slug: communicate-so
slug: communicate-so-agentic-access
source_filename: communicate-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/communicate-so-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 270\n  by_action_class:\n    acting: 186\n    connected: 84\n  by_consequence:\n    write: 150\n    read: 84\n    safety-critical: 10\n    physical: 26\n  human_in_the_loop_required: 10\noperations:\n- path: /account-credentials/bootstrap\n  method: post\n  operationId: bootstrapAccountCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-credentials\n  method:\
  \ post\n  operationId: createAccountCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-credentials\n  method: get\n  operationId: listAccountCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-credentials/{credentialId}\n  method: patch\n  operationId: editAccountCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-credentials/{credentialId}\n  method: delete\n  operationId:\
  \ revokeAccountCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account-credentials/{credentialId}/rotate\n  method: post\n  operationId: rotateAccountCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: post\n  operationId: createWorkspace\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/preferences\n  method: get\n  operationId: getAccountPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/preferences\n  method: patch\n  operationId: updateAccountPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: delete\n  operationId: removeContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: get\n  operationId: readContactProfile\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: patch\n  operationId: updateContactProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/support-requests/live\n  method: get\n  operationId: listInboxLiveSupportRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/copilot\n  method: post\n  operationId: requestInboxCopilotSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/copilot/endorse\n  method: post\n  operationId: endorseInboxCopilotLearning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/attachments/presign\n  method: post\n  operationId: presignInboxAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/attachments/confirm\n  method: post\n  operationId: confirmInboxAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/attachments/{attachmentId}/url\n  method: get\n  operationId: readInboxAttachmentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/messages/{messageId}/retry\n  method: post\n  operationId: retryInboxReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/merge\n  method: post\n  operationId: mergeSupportRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/{requestId}/split\n  method: post\n  operationId: splitSupportRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/{requestId}/transitions\n\
  \  method: post\n  operationId: transitionSupportRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/{requestId}/evidence\n  method: post\n  operationId: appendSupportRequestEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/{requestId}/sla/bind\n  method: post\n  operationId: bindSupportRequestSla\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/{requestId}/sla/milestones\n  method: post\n  operationId: recordSupportRequestSlaMilestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/support-requests/{requestId}/sla/clocks/{kind}\n  method: get\n  operationId: readSupportRequestSlaClock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/labels\n  method: get\n  operationId: listWorkspaceLabels\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/labels\n  method: post\n  operationId: createWorkspaceLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/labels/{labelId}\n  method: patch\n  operationId: updateWorkspaceLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/labels/{labelId}\n  method: delete\n  operationId: deleteWorkspaceLabel\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/labels/{labelId}\n  method: post\n  operationId: attachInboxLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/labels/{labelId}\n  method: delete\n  operationId: detachInboxLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/notes\n  method: post\n  operationId: createInboxNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/read\n  method: post\n  operationId: markInboxConversationRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}\n  method: get\n  operationId: readInboxConversation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/inbox/{conversationId}\n  method: patch\n  operationId: updateInboxConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/messages/{messageId}\n  method: patch\n  operationId: editInboxReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/messages/{messageId}/undo\n  method: post\n  operationId: undoInboxReply\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox/{conversationId}/messages\n  method: post\n  operationId: sendInboxReply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/inbox\n  method: get\n  operationId: listInboxConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/inbox/counts\n\
  \  method: get\n  operationId: readInboxCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations\n  method: get\n  operationId: listLinkedConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/counts\n  method: get\n  operationId: countLinkedConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}\n  method: get\n  operationId: readLinkedConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}\n  method: patch\n  operationId: setLinkedConversationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/read\n  method: post\n  operationId: markLinkedConversationRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/copilot\n  method: post\n  operationId: requestLinkedCopilotSuggestion\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/copilot/endorse\n  method: post\n  operationId: endorseLinkedCopilotLearning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/attachments/presign\n  method: post\n  operationId: presignLinkedAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/attachments/confirm\n  method: post\n  operationId: confirmLinkedAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/attachments/{attachmentId}/url\n  method: get\n  operationId: readLinkedAttachmentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/messages\n\
  \  method: post\n  operationId: sendLinkedConversationReply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/messages/{messageId}/undo\n  method: post\n  operationId: undoLinkedConversationReply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/messages/{messageId}\n\
  \  method: patch\n  operationId: editLinkedConversationReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/messages/{messageId}/retry\n  method: post\n  operationId: retryLinkedConversationReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/notes\n  method: post\n  operationId: addLinkedConversationNote\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/labels/{labelId}\n  method: post\n  operationId: addLinkedConversationLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/labels/{labelId}\n  method: delete\n  operationId: removeLinkedConversationLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/assign\n  method: post\n  operationId: assignLinkedConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/takeover\n  method: post\n  operationId: takeOverLinkedConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{destinationWorkspaceId}/linked-conversations/{conversationId}/actions/{actionId}/run\n\
  \  method: post\n  operationId: runLinkedConversationAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/conversations\n  method: post\n  operationId: startConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /workspaces/{workspaceId}/conversations/{conversationId}\n  method: get\n  operationId: readConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/conversations/{conversationId}\n  method: patch\n  operationId: setConversationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: get\n  operationId: readWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}\n  method: patch\n  operationId: updateWorkspace\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/members\n  method: get\n  operationId: listWorkspaceMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/members\n  method: post\n  operationId: addWorkspaceMember\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/members/{memberId}\n  method: patch\n  operationId: updateWorkspaceMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/members/{memberId}\n  method: delete\n  operationId: removeWorkspaceMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /workspaces/{workspaceId}/members/invites\n  method: get\n  operationId: listWorkspaceInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/members/invites\n  method: post\n  operationId: createWorkspaceInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/members/invites/{inviteId}/resend\n  method: post\n  operationId: resendWorkspaceInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/members/invites/{inviteId}\n  method: delete\n  operationId: cancelWorkspaceInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites/{token}/accept\n  method: post\n  operationId: acceptWorkspaceInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/members/{memberId}/agents\n  method: get\n  operationId: readMemberAgentAccess\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/members/{memberId}/agents\n  method: put\n  operationId: updateMemberAgentAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/teams/{teamId}\n  method: patch\n  operationId: updateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/teams/{teamId}\n  method: delete\n  operationId: deleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/teams/{teamId}/members\n  method: post\n  operationId: addTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/teams/{teamId}/members/{memberId}\n  method: delete\n  operationId: removeTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/custom-domains\n  method: get\n  operationId: listCustomDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/custom-domains\n  method: post\n  operationId: createCustomDomain\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/custom-domains/{domainId}/verify\n  method: post\n  operationId: verifyCustomDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (92 KB total) ---\n# Full source: https://artifacts.apis.io/communicate-so/agentic-access/communicate-so-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/communicate-so/agentic-access/communicate-so-agentic-access.yml
summary_line: 270 operations · 186 acting · 10 human-in-the-loop
tags:
- Artificial Intelligence
- Customer Service
- Chatbots
- Software-as-a-Service
- Automation
---
