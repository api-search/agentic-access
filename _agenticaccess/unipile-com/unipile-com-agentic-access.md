---
acting_count: 45
action_class_counts:
  acting: 45
  connected: 53
api_specs:
- filename: unipile-com-accounts-api-openapi.yml
  format: yaml
  label: unipile-com Accounts API
  slug: unipile-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-accounts-api-openapi.yml
- filename: unipile-com-calendars-api-openapi.yml
  format: yaml
  label: unipile-com Calendars API
  slug: unipile-com-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-calendars-api-openapi.yml
- filename: unipile-com-emails-api-openapi.yml
  format: yaml
  label: unipile-com Emails API
  slug: unipile-com-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-emails-api-openapi.yml
- filename: unipile-com-linkedin-specific-api-openapi.yml
  format: yaml
  label: unipile-com LinkedIn Specific API
  slug: unipile-com-linkedin-specific-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-linkedin-specific-api-openapi.yml
- filename: unipile-com-messaging-api-openapi.yml
  format: yaml
  label: unipile-com Messaging API
  slug: unipile-com-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-messaging-api-openapi.yml
- filename: unipile-com-posts-api-openapi.yml
  format: yaml
  label: unipile-com Posts API
  slug: unipile-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-posts-api-openapi.yml
- filename: unipile-com-users-api-openapi.yml
  format: yaml
  label: unipile-com Users API
  slug: unipile-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-users-api-openapi.yml
- filename: unipile-com-webhooks-api-openapi.yml
  format: yaml
  label: unipile-com Webhooks API
  slug: unipile-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unipile-com/openapi/unipile-com-webhooks-api-openapi.yml
consequence_counts:
  read: 53
  safety-critical: 45
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 45
kind: agentic-access
layout: agentic-access
method: generated
name: Unipile Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/accounts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/accounts/checkpoint
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/accounts/checkpoint/resend
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/accounts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/accounts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/accounts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/accounts/{id}/restart
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/calendars/{calendar_id}/events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/calendars/{calendar_id}/events/{event_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/calendars/{calendar_id}/events/{event_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/chats
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/chats/{chat_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/chats/{chat_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/chats/{chat_id}/messages
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/drafts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/emails
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/emails/{email_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/emails/{email_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/hosted/accounts/link
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/linkedin/contracts/{id}/select
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/linkedin/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/linkedin/jobs/{draft_id}/checkpoint
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/linkedin/jobs/{draft_id}/publish
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/linkedin/jobs/{id}/close
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/linkedin/jobs/{job_id}
operation_count: 98
overview: 'unipile-com exposes 98 API operations that an AI agent could call, of which 45 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 53 read and 45 safety-critical.


  45 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: unipile-com
provider_slug: unipile-com
slug: unipile-com-agentic-access
source_filename: unipile-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/unipile-com-api-reference-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 98\n  by_action_class:\n    connected: 53\n    acting: 45\n  by_consequence:\n    read: 53\n    safety-critical: 45\n  human_in_the_loop_required: 45\noperations:\n- path: /api/v1/accounts\n  method: get\n  operationId: AccountsController_listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts\n  method: post\n  operationId: AccountsController_createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/accounts/checkpoint\n  method: post\n  operationId: AccountsController_solveCheckpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/accounts/checkpoint/resend\n  method: post\n  operationId: AccountsController_resendCheckpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v1/accounts/{account_id}/sync\n  method: get\n  operationId: AccountsController_resyncAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{id}\n  method: get\n  operationId: AccountsController_getAccountById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts/{id}\n  method: post\n  operationId: AccountsController_reconnectAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/accounts/{id}\n  method: delete\n  operationId:\
  \ AccountsController_deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/accounts/{id}\n  method: patch\n  operationId: AccountsController_patchAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/accounts/{id}/restart\n  method: post\n  operationId: AccountsController_restartAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/calendars\n  method: get\n  operationId: CalendarsController_listCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars/{calendar_id}\n  method: get\n  operationId: CalendarsController_getCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars/{calendar_id}/events\n  method: get\n  operationId: CalendarsController_listCalendarEventsByCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars/{calendar_id}/events\n  method: post\n\
  \  operationId: CalendarsController_createCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/calendars/{calendar_id}/events/{event_id}\n  method: get\n  operationId: CalendarsController_getCalendarEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars/{calendar_id}/events/{event_id}\n  method: patch\n  operationId: CalendarsController_editCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/calendars/{calendar_id}/events/{event_id}\n  method: delete\n  operationId: CalendarsController_deleteCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/chat_attendees\n  method: get\n  operationId: ChatAttendeesController_listAllAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat_attendees/{attendee_id}/chats\n  method: get\n  operationId: ChatAttendeesController_listChatsByAttendee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat_attendees/{attendee_id}/sync\n  method: get\n  operationId: ChatAttendeesController_syncAttendeeHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat_attendees/{id}\n  method: get\n  operationId: ChatAttendeesController_getAttendeeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat_attendees/{id}/picture\n  method: get\n  operationId: ChatAttendeesController_getAttendeeProfilePicture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chat_attendees/{sender_id}/messages\n  method: get\n  operationId: ChatAttendeesController_listMessagesByAttendee\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chats\n  method: get\n  operationId: ChatsController_listAllChats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chats\n  method: post\n  operationId: ChatsController_startNewChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/chats/{chat_id}\n  method: get\n  operationId: ChatsController_getChat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chats/{chat_id}\n\
  \  method: patch\n  operationId: ChatsController_patchChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/chats/{chat_id}\n  method: delete\n  operationId: ChatsController_deleteChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/chats/{chat_id}/attendees\n  method: get\n  operationId: ChatsController_listAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/chats/{chat_id}/messages\n  method: get\n  operationId: ChatsController_listChatMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chats/{chat_id}/messages\n  method: post\n  operationId: ChatsController_sendMessageInChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/chats/{chat_id}/sync\n  method: get\n  operationId: ChatsController_syncChatHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/drafts\n  method: post\n  operationId:\
  \ DraftsController_createDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/emails\n  method: get\n  operationId: MailsController_listMails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/emails\n  method: post\n  operationId: MailsController_sendMail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/emails/contacts\n\
  \  method: get\n  operationId: MailsController_listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/emails/{email_id}\n  method: get\n  operationId: MailsController_getMail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/emails/{email_id}\n  method: delete\n  operationId: MailsController_deleteMail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/emails/{email_id}\n  method: put\n  operationId: MailsController_updateMail\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/emails/{email_id}/attachments/{attachment_id}\n  method: get\n  operationId: MailsController_getAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/folders\n  method: get\n  operationId: FoldersController_listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/folders/{folder_id}\n  method: get\n  operationId: FoldersController_getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/hosted/accounts/link\n  method: post\n  operationId: HostedController_requestLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin\n  method: post\n  operationId: LinkedinController_getRawData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/company/{identifier}\n  method: get\n  operationId: LinkedinController_getCompanyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/contracts\n  method: get\n  operationId: LinkedinController_getAvailableContracts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/contracts/{id}/select\n  method: post\n  operationId: LinkedinController_selectContract\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/inmail_balance\n  method: get\n  operationId: LinkedinController_getInmailBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/jobs\n  method: get\n  operationId: LinkedinController_getJobPostings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/jobs\n  method: post\n  operationId: LinkedinController_createJobPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/jobs/applicants/{applicant_id}\n  method: get\n  operationId: LinkedinController_getJobApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/jobs/applicants/{applicant_id}/resume\n  method: get\n  operationId: LinkedinController_getJobApplicantResume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/jobs/{draft_id}/checkpoint\n  method: post\n  operationId: LinkedinController_solveCheckpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/jobs/{draft_id}/publish\n  method: post\n  operationId: LinkedinController_publishJobPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/jobs/{id}/applicants\n  method: get\n  operationId: LinkedinController_getJobApplicants\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/jobs/{id}/close\n  method: post\n  operationId: LinkedinController_closeJobPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/jobs/{job_id}\n  method: get\n  operationId: LinkedinController_getJobPosting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/jobs/{job_id}\n  method: patch\n  operationId: LinkedinController_editJobPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/posts/targeted-audience\n  method: post\n  operationId: LinkedinController_getPostTargetAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/profile/endorse\n  method: post\n  operationId: LinkedinController_endorseProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/projects\n  method: get\n  operationId: LinkedinController_getHiringProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/projects/{id}\n  method: get\n  operationId: LinkedinController_getHiringProjectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/recruiter/sessions/signout\n  method: post\n  operationId: LinkedinController_signOutRecruiterSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/v1/linkedin/recruiter/sessions/signout-others\n  method: post\n  operationId: LinkedinController_signOutOtherRecruiterSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/search\n  method: post\n  operationId: LinkedinController_search\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/linkedin/search/parameters\n  method: get\n  operationId: LinkedinController_getSearchParametersList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linkedin/user/{user_id}\n  method: post\n  operationId: LinkedinController_performActionOnMember\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/messages\n  method: get\n  operationId: MessagesController_listAllMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/messages/{message_id}\n  method: get\n  operationId: MessagesController_getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/messages/{message_id}\n  method: delete\n  operationId: MessagesController_deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/messages/{message_id}\n  method: patch\n  operationId: MessagesController_patchMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/messages/{message_id}/attachments/{attachment_id}\n  method: get\n  operationId: MessagesController_getAttachment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/messages/{message_id}/forward\n  method: post\n  operationId: MessagesController_forwardMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/messages/{message_id}/reaction\n  method: post\n  operationId: MessagesController_addReaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/v1/messages/{message_id}/reaction\n  method: delete\n  operationId: MessagesController_removeReaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/posts\n  method: post\n  operationId: PostsController_createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/posts/reaction\n  method: post\n  operationId: PostsController_addPostReaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/posts/{post_id}\n  method: get\n  operationId: PostsController_getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts/{post_id}/comments\n  method: get\n  operationId: PostsController_listAllComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts/{post_id}/comments\n  method: post\n  operationId: PostsController_sendComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/posts/{post_id}/reactions\n  method: get\n  operationId: PostsController_listAllReactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/followers\n  method: get\n  operationId: UsersController_getFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/following\n  method: get\n  operationId: UsersController_getFollowing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/invite\n  method: post\n  operationId: UsersController_addUserByIdentifier\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/users/invite/received\n  method: get\n  operationId: UsersController_listAllUserInvitationsReceived\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/invite/received/{invitation_id}\n  method: post\n  operationId: UsersController_handleInvitationReceived\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/users/invite/sent\n\
  \  method: get\n  operationId: UsersController_listAllUserInvitationsSent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/invite/sent/{invitation_id}\n  method: delete\n  operationId: UsersController_cancelInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/users/me\n  method: get\n  operationId: UsersController_getAccountOwnerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/edit\n  method: patch\n  operationId: UsersController_editAccountOwnerProfile\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/users/relations\n  method: get\n  operationId: UsersController_getRelations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/{identifier}\n  method: get\n  operationId: UsersController_getProfileByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/{identifier}/comments\n  method: get\n  operationId: UsersController_listAllComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/{identifier}/posts\n  method: get\n  operationId: UsersController_listAllPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/{identifier}/reactions\n  method: get\n  operationId: UsersController_listAllReactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: get\n  operationId: WebhooksController_listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: WebhooksController_createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: delete\n  operationId: WebhooksController_deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/unipile-com/agentic-access/unipile-com-agentic-access.yml
summary_line: 98 operations · 45 acting · 45 human-in-the-loop
tags:
- Messaging
- Integration
- Multi-Channel
- Communications
---
