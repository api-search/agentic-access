---
acting_count: 45
action_class_counts:
  acting: 45
  connected: 29
api_specs:
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Agents API
  slug: chatwoot-application-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Teams API
  slug: chatwoot-application-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Inboxes API
  slug: chatwoot-application-inboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Contacts API
  slug: chatwoot-application-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Conversations API
  slug: chatwoot-application-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Messages API
  slug: chatwoot-application-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Labels API
  slug: chatwoot-application-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Custom Attributes API
  slug: chatwoot-application-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Canned Responses API
  slug: chatwoot-application-canned-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Automation Rules API
  slug: chatwoot-application-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Reports API
  slug: chatwoot-application-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Client Contacts API
  slug: chatwoot-client-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Client Conversations API
  slug: chatwoot-client-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Client Messages API
  slug: chatwoot-client-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Platform Users API
  slug: chatwoot-platform-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Platform Accounts API
  slug: chatwoot-platform-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Platform Agent Bots API
  slug: chatwoot-platform-agent-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
consequence_counts:
  read: 29
  write: 45
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chatwoot Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 74
overview: 'Chatwoot exposes 74 API operations that an AI agent could call, of which 45 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 45 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chatwoot
provider_slug: chatwoot-com
slug: chatwoot-com-agentic-access
source_filename: chatwoot-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chatwoot-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 74\n  by_action_class:\n    connected: 29\n    acting: 45\n  by_consequence:\n    read: 29\n    write: 45\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/accounts/{account_id}/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/agents\n  method: post\n  operationId: addAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/agents/{id}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/agents/{id}\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/teams/{team_id}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/teams/{team_id}\n  method: patch\n  operationId: updateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/teams/{team_id}\n  method: delete\n  operationId: deleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/inboxes\n  method: get\n  operationId: listInboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/inboxes/{id}\n  method: get\n  operationId: getInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/inboxes/{id}\n  method:\
  \ patch\n  operationId: updateInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/inboxes/{id}\n  method: delete\n  operationId: deleteInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/contacts\n  method: post\n  operationId:\
  \ createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/contacts/search\n  method: get\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/contacts/filter\n  method: post\n  operationId: filterContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/contacts/{id}\n  method: get\n  operationId:\
  \ getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/contacts/{id}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/contacts/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/contacts/{id}/conversations\n  method: get\n  operationId:\
  \ listContactConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/conversations\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/conversations\n  method: post\n  operationId: createConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/toggle_status\n  method: post\n  operationId: toggleConversationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/assignments\n  method: post\n  operationId: assignConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/labels\n  method: get\n  operationId:\
  \ getConversationLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/labels\n  method: post\n  operationId: setConversationLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/conversations/{conversation_id}/messages/{message_id}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/labels\n  method: get\n  operationId: listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/custom_attribute_definitions\n  method: get\n  operationId:\
  \ listCustomAttributeDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/custom_attribute_definitions\n  method: post\n  operationId: createCustomAttributeDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/custom_attribute_definitions/{id}\n  method: patch\n  operationId: updateCustomAttributeDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/accounts/{account_id}/custom_attribute_definitions/{id}\n  method: delete\n  operationId: deleteCustomAttributeDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/canned_responses\n  method: get\n  operationId: listCannedResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/canned_responses\n  method: post\n  operationId: createCannedResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/canned_responses/{id}\n  method: patch\n  operationId: updateCannedResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/canned_responses/{id}\n  method: delete\n  operationId: deleteCannedResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/automation_rules\n  method: get\n  operationId: listAutomationRules\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/automation_rules\n  method: post\n  operationId: createAutomationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/automation_rules/{id}\n  method: get\n  operationId: getAutomationRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/automation_rules/{id}\n  method: patch\n  operationId: updateAutomationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/automation_rules/{id}\n  method: delete\n  operationId: deleteAutomationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/accounts/{account_id}/reports\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{account_id}/conversations/meta\n  method: get\n  operationId: getConversationReportsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts\n  method: post\n  operationId: createClientContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}\n  method: get\n  operationId: getClientContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}\n  method: patch\n  operationId: updateClientContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations\n  method: get\n  operationId: listClientConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations\n  method: post\n  operationId: createClientConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations/{conversation_id}/toggle_status\n  method: post\n  operationId: toggleClientConversationStatus\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations/{conversation_id}/toggle_typing\n  method: post\n  operationId: toggleClientTyping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations/{conversation_id}/update_last_seen\n  method: post\n  operationId: updateClientLastSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations/{conversation_id}/messages\n  method: get\n  operationId: listClientMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/api/v1/inboxes/{inbox_identifier}/contacts/{contact_identifier}/conversations/{conversation_id}/messages\n  method: post\n  operationId: createClientMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/users\n  method:\
  \ post\n  operationId: createPlatformUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/users/{id}\n  method: get\n  operationId: getPlatformUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/api/v1/users/{id}\n  method: patch\n  operationId: updatePlatformUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/users/{id}\n  method: delete\n  operationId: deletePlatformUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/users/{id}/login\n  method: get\n  operationId: getPlatformUserLoginLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/api/v1/accounts\n  method: post\n  operationId: createPlatformAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/accounts/{account_id}\n  method: get\n  operationId: getPlatformAccount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/api/v1/accounts/{account_id}\n  method: patch\n  operationId: updatePlatformAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/accounts/{account_id}\n  method: delete\n  operationId: deletePlatformAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/accounts/{account_id}/account_users\n  method: get\n  operationId: listPlatformAccountUsers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/api/v1/accounts/{account_id}/account_users\n  method: post\n  operationId: createPlatformAccountUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/accounts/{account_id}/account_users\n  method: delete\n  operationId: deletePlatformAccountUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/agent_bots\n  method: get\n  operationId:\
  \ listPlatformAgentBots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/api/v1/agent_bots\n  method: post\n  operationId: createPlatformAgentBot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/agent_bots/{id}\n  method: get\n  operationId: getPlatformAgentBot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/api/v1/agent_bots/{id}\n  method: patch\n  operationId: updatePlatformAgentBot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/api/v1/agent_bots/{id}\n  method: delete\n  operationId: deletePlatformAgentBot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/agentic-access/chatwoot-com-agentic-access.yml
summary_line: 74 operations · 45 acting
tags:
- Customer Support
- Customer Engagement
- Shared Inbox
- Live Chat
- Open Source
- Omnichannel
- Help Desk
---
