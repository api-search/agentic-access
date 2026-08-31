---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 25
api_specs:
- filename: spruce-health-contact-fields-api-openapi.yml
  format: yaml
  label: Spruce Health Contact Fields API
  slug: spruce-health-contact-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contact-fields-api-openapi.yml
- filename: spruce-health-contact-tags-api-openapi.yml
  format: yaml
  label: Spruce Health Contact Tags API
  slug: spruce-health-contact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contact-tags-api-openapi.yml
- filename: spruce-health-contacts-api-openapi.yml
  format: yaml
  label: Spruce Health Contacts API
  slug: spruce-health-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contacts-api-openapi.yml
- filename: spruce-health-conversation-item-api-openapi.yml
  format: yaml
  label: Spruce Health Conversation Item API
  slug: spruce-health-conversation-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversation-item-api-openapi.yml
- filename: spruce-health-conversation-tags-api-openapi.yml
  format: yaml
  label: Spruce Health Conversation Tags API
  slug: spruce-health-conversation-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversation-tags-api-openapi.yml
- filename: spruce-health-conversations-api-openapi.yml
  format: yaml
  label: Spruce Health Conversations API
  slug: spruce-health-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversations-api-openapi.yml
- filename: spruce-health-internal-endpoints-api-openapi.yml
  format: yaml
  label: Spruce Health Internal Endpoints API
  slug: spruce-health-internal-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-internal-endpoints-api-openapi.yml
- filename: spruce-health-media-api-openapi.yml
  format: yaml
  label: Spruce Health Media API
  slug: spruce-health-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-media-api-openapi.yml
- filename: spruce-health-organization-api-openapi.yml
  format: yaml
  label: Spruce Health Organization API
  slug: spruce-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-organization-api-openapi.yml
- filename: spruce-health-phone-lines-api-openapi.yml
  format: yaml
  label: Spruce Health Phone Lines API
  slug: spruce-health-phone-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-phone-lines-api-openapi.yml
- filename: spruce-health-saved-messages-api-openapi.yml
  format: yaml
  label: Spruce Health Saved Messages API
  slug: spruce-health-saved-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-saved-messages-api-openapi.yml
- filename: spruce-health-scheduled-messages-api-openapi.yml
  format: yaml
  label: Spruce Health Scheduled Messages API
  slug: spruce-health-scheduled-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-scheduled-messages-api-openapi.yml
- filename: spruce-health-teams-api-openapi.yml
  format: yaml
  label: Spruce Health Teams API
  slug: spruce-health-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-teams-api-openapi.yml
- filename: spruce-health-transcription-api-openapi.yml
  format: yaml
  label: Spruce Health Transcription API
  slug: spruce-health-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-transcription-api-openapi.yml
- filename: spruce-health-webhooks-api-openapi.yml
  format: yaml
  label: Spruce Health Webhooks API
  slug: spruce-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 25
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spruce Health Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contacts/{contactId}/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /internalendpoints/{internalEndpointId}/conversations
operation_count: 47
overview: 'Spruce Health exposes 47 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 20 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spruce Health
provider_slug: spruce-health
slug: spruce-health-agentic-access
source_filename: spruce-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: generated\nsource: openapi/spruce-health-contact-fields-openapi.yml, openapi/spruce-health-contact-tags-openapi.yml,\n  openapi/spruce-health-contacts-openapi.yml, openapi/spruce-health-conversation-item-openapi.yml,\n  openapi/spruce-health-conversation-tags-openapi.yml, openapi/spruce-health-conversations-openapi.yml,\n  openapi/spruce-health-internal-endpoints-openapi.yml, openapi/spruce-health-media-openapi.yml,\n  openapi/spruce-health-organization-openapi.yml, openapi/spruce-health-phone-lines-openapi.yml,\n  openapi/spruce-health-saved-messages-openapi.yml, openapi/spruce-health-scheduled-messages-openapi.yml,\n  openapi/spruce-health-teams-openapi.yml, openapi/spruce-health-transcription-openapi.yml,\n  openapi/spruce-health-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n\
  \  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 25\n    acting: 22\n  by_consequence:\n    read: 25\n    write: 20\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /contacts/fields\n  method: get\n  operationId: ContactFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/fields\n  method: post\n  operationId: CreateContactField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/tags\n  method: get\n  operationId: ContactTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/tags\n  method: post\n  operationId: CreateContactTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: ListContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: CreateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}\n  method: delete\n\
  \  operationId: DeleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}\n  method: get\n  operationId: Contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}\n  method: patch\n  operationId: UpdateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}/conversations\n  method: get\n  operationId: ContactConversations\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}/integrationlinks\n  method: delete\n  operationId: DeleteContactIntegrationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}/integrationlinks\n  method: get\n  operationId: ContactIntegrationLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}/integrationlinks\n  method: post\n  operationId: CreateContactIntegrationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}/invite\n  method: post\n  operationId: SendInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/search\n  method: post\n  operationId: SearchContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversationItems/{conversationItemId}\n  method: delete\n  operationId: DeleteConversationItem\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversationItems/{conversationItemId}\n  method: get\n  operationId: ConversationItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/tags\n  method: get\n  operationId: ConversationTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/tags\n  method: post\n  operationId: CreateConversationTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations\n  method: get\n  operationId: ListConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations\n  method: post\n  operationId: CreateConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationId}\n  method: get\n  operationId: Conversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversationId}\n  method: patch\n  operationId: UpdateConversation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationId}/items\n  method: get\n  operationId: ConversationItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversationId}/messages\n  method: post\n  operationId: PostConversationMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internalendpoints\n  method: get\n  operationId: InternalEndpoints\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internalendpoints/{internalEndpointId}/calls\n  method: post\n  operationId: PostCreateProxyCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internalendpoints/{internalEndpointId}/conversations\n  method: post\n  operationId: PostMessageFromEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media\n  method: post\n  operationId: UploadMedia\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization\n  method: get\n  operationId: Organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/members\n  method: get\n  operationId: OrganizationMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/members/{memberId}\n  method: get\n  operationId: OrganizationMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonelines\n  method: get\n  operationId: PhoneLines\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonelines/{phonelineId}\n  method: get\n  operationId: PhoneLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /savedmessages\n  method: get\n  operationId: ListSavedMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversationId}/scheduledmessages\n  method: get\n  operationId: ListConversationScheduledMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversationId}/scheduledmessages\n  method: post\n  operationId: ScheduleConversationMessage\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduledmessages\n  method: get\n  operationId: ListScheduledMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduledmessages/{scheduledMessageId}\n  method: delete\n  operationId: DeleteScheduledMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{teamId}/members\n  method: get\n  operationId: TeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transcriptions/{transcriptionId}\n  method: get\n  operationId: Transcription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints\n  method: get\n  operationId: ListWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints\n  method: post\n  operationId: CreateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints/{endpointId}\n  method: delete\n  operationId: DeleteWebhookEndpoint\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/endpoints/{endpointId}\n  method: get\n  operationId: WebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints/{endpointId}/events\n  method: get\n  operationId: ListWebhookEndpointEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/endpoints/{endpointId}/paused\n  method: post\n  operationId: ModifyWebhookEndpointPaused\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/agentic-access/spruce-health-agentic-access.yml
summary_line: 47 operations · 22 acting
tags:
- Healthcare
- HIPAA
- Communications
- Secure Messaging
- Telehealth
- Patient Engagement
- Contacts
- Conversations
- Messaging
- SMS
- Voice
- VoIP
- Fax
- Video
- Webhook
- Scheduling
- Transcription
- EHR Integration
- Compliance
---
