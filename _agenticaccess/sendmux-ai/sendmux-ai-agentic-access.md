---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 69
api_specs:
- filename: sendmux-ai-billing-api-openapi.yml
  format: yaml
  label: sendmux-ai Billing API
  slug: sendmux-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-billing-api-openapi.yml
- filename: sendmux-ai-connection-api-openapi.yml
  format: yaml
  label: sendmux-ai Connection API
  slug: sendmux-ai-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-connection-api-openapi.yml
- filename: sendmux-ai-domain-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Domain Filters API
  slug: sendmux-ai-domain-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domain-filters-api-openapi.yml
- filename: sendmux-ai-domains-api-openapi.yml
  format: yaml
  label: sendmux-ai Domains API
  slug: sendmux-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domains-api-openapi.yml
- filename: sendmux-ai-emails-api-openapi.yml
  format: yaml
  label: sendmux-ai Emails API
  slug: sendmux-ai-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-emails-api-openapi.yml
- filename: sendmux-ai-inboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Inboxes API
  slug: sendmux-ai-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-inboxes-api-openapi.yml
- filename: sendmux-ai-mailbox-api-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox API
  slug: sendmux-ai-mailbox-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-api-api-openapi.yml
- filename: sendmux-ai-mailbox-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox Filters API
  slug: sendmux-ai-mailbox-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-filters-api-openapi.yml
- filename: sendmux-ai-mailboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailboxes API
  slug: sendmux-ai-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailboxes-api-openapi.yml
- filename: sendmux-ai-sending-accounts-api-openapi.yml
  format: yaml
  label: sendmux-ai Sending accounts API
  slug: sendmux-ai-sending-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-sending-accounts-api-openapi.yml
- filename: sendmux-ai-webhooks-api-openapi.yml
  format: yaml
  label: sendmux-ai Webhooks API
  slug: sendmux-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 19
  read: 69
  safety-critical: 2
  write: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Sendmux Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /mailbox/drafts/{draftId}/schedule
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /mailboxes/{public_id}/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /domains/{public_id}/filters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /mailbox-send-policies/{scope}/{public_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mailbox/calendar-events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /mailbox/calendar-events/{event_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /mailbox/calendar-events/{event_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mailbox/drafts/{draftId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /mailbox/identity
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mailbox/messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /mailboxes/{public_id}/filters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /providers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /providers/limits/sending-accounts/request-increase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /providers/shared-amazon-ses-limit-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /providers/shared-amazon-ses-limit-request/{request_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /providers/{public_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /providers/{public_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /providers/{public_id}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /providers/{public_id}/deactivate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /providers/{public_id}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{public_id}/test
operation_count: 119
overview: 'sendmux-ai exposes 119 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 69 read, 29 write, 19 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sendmux-ai
provider_slug: sendmux-ai
slug: sendmux-ai-agentic-access
source_filename: sendmux-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/openapi-app.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 119\n  by_action_class:\n    connected: 69\n    acting: 50\n  by_consequence:\n    read: 69\n    write: 29\n    physical: 19\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /billing/balance\n  method: get\n  operationId: managementListBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/summary\n  method: get\n  operationId: managementGetSpendSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - billing.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/transactions\n  method: get\n  operationId: managementListTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: get\n  operationId: managementListDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - domain.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: post\n  operationId: managementCreateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - domain.create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{public_id}\n\
  \  method: delete\n  operationId: managementDeleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - domain.delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{public_id}\n  method: get\n  operationId: managementGetDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - domain.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{public_id}\n  method: patch\n  operationId: managementUpdateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - domain.create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /domains/{public_id}/filters\n  method: get\n  operationId: managementGetDomainFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.admin.manage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{public_id}/filters\n  method: put\n  operationId: managementSetDomainFilters\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{public_id}/verify\n  method: post\n  operationId: managementVerifyDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - domain.verify\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{public_id}/zone-file\n  method: get\n  operationId: managementGetDomainZoneFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - domain.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/logs\n  method: get\n  operationId: managementListEmailLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - logs.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/logs/{public_id}\n  method: get\n  operationId: managementGetEmailLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - logs.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/metrics\n  method: get\n\
  \  operationId: managementGetEmailMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - analytics.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/logs\n  method: get\n  operationId: managementListInboxLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - logs.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/logs/{public_id}\n  method: get\n  operationId: managementGetInboxLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - logs.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox-send-policies/{scope}/{public_id}\n  method: get\n  operationId: managementGetMailboxSendPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - key.read\n    - mailbox.admin.read\n\
  \    - team.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox-send-policies/{scope}/{public_id}\n  method: put\n  operationId: managementReplaceMailboxSendPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - key.*\n    - mailbox.admin.manage\n    - team.update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/attachment-uploads\n  method: post\n  operationId: mailboxCreateAttachmentUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email.send\n    - mailbox.drafts.write\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /mailbox/attachments:upload\n  method: post\n  operationId: mailboxUploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email.send\n    - mailbox.drafts.write\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/calendar-events\n  method: get\n  operationId: mailboxListCalendarEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - calendar.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/calendar-events\n  method: post\n  operationId: mailboxCreateCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - calendar.write\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/calendar-events/{event_id}\n  method: delete\n  operationId: mailboxDeleteCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - calendar.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/calendar-events/{event_id}\n  method: get\n  operationId: mailboxGetCalendarEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - calendar.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/calendar-events/{event_id}\n\
  \  method: patch\n  operationId: mailboxUpdateCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - calendar.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/calendar-events/changes\n  method: get\n  operationId: mailboxGetCalendarEventChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - calendar.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/calendars\n  method: get\n  operationId: mailboxListCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - calendar.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/calendars\n  method:\
  \ post\n  operationId: mailboxCreateCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - calendar.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/calendars/{calendar_id}\n  method: get\n  operationId: mailboxGetCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - calendar.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/changes\n  method: get\n  operationId: mailboxGetChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/connection\n  method: get\n  operationId: mailboxGetConnection\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/drafts\n  method: get\n  operationId: mailboxListDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/drafts\n  method: post\n  operationId: mailboxCreateDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.drafts.write\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/drafts/{draftId}\n  method: delete\n  operationId: mailboxDeleteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.drafts.write\n   \
  \ - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/drafts/{draftId}\n  method: get\n  operationId: mailboxGetDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/drafts/{draftId}\n  method: patch\n  operationId: mailboxUpdateDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.drafts.write\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/drafts/{draftId}/schedule\n  method: patch\n  operationId: mailboxControlDraftSchedule\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - email.send\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mailbox/drafts/{draftId}/send\n  method: post\n  operationId: mailboxSendDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - email.send\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/events\n  method: get\n  operationId: mailboxStreamEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/folders\n  method: get\n  operationId: mailboxListFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/folders\n  method: post\n  operationId: mailboxCreateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/folders/{folder_id}\n  method: delete\n  operationId: mailboxDeleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/folders/{folder_id}\n  method: get\n  operationId: mailboxGetFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/folders/{folder_id}\n  method: patch\n  operationId: mailboxUpdateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/folders/changes\n  method: get\n  operationId: mailboxGetFolderChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/folders/query-changes\n  method: get\n  operationId: mailboxQueryFolderChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/identities\n  method: get\n  operationId: mailboxListIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/identity\n  method: get\n  operationId: mailboxGetIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/identity\n  method: patch\n  operationId: mailboxUpdateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/mailboxes\n  method: get\n  operationId: mailboxListGrantedMailboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/me\n  method: get\n  operationId: mailboxGetMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages\n  method: get\n  operationId: mailboxListMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages:batch-delete\n  method: post\n  operationId: mailboxBatchDeleteMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/messages:batch-get\n  method: post\n  operationId: mailboxBatchGetMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/messages:batch-update\n  method: post\n  operationId: mailboxBatchUpdateMessages\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/messages/{message_id}\n  method: delete\n  operationId: mailboxDeleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/messages/{message_id}\n  method: get\n  operationId: mailboxGetMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/{message_id}\n  method:\
  \ patch\n  operationId: mailboxUpdateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.settings.update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/messages/{message_id}/attachments/{attachment_id}\n  method: get\n  operationId: mailboxGetMessageAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/{message_id}/attachments/{attachment_id}/text\n  method: get\n  operationId: mailboxGetAttachmentText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/{message_id}/attachments/{attachment_id}/text\n\
  \  method: post\n  operationId: mailboxRequestAttachmentText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/messages/{message_id}/body\n  method: get\n  operationId: mailboxListBody\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/{message_id}/content\n  method: get\n  operationId: mailboxListContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/{message_id}/raw\n  method: get\n  operationId: mailboxDownloadRawMessage\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/count\n  method: get\n  operationId: mailboxCountMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/query-changes\n  method: get\n  operationId: mailboxQueryMessageChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/messages/search-snippets\n  method: get\n  operationId: mailboxSearchMessageSnippets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /mailbox/messages/send\n  method: post\n  operationId: mailboxSendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - email.send\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailbox/quotas\n  method: get\n  operationId: mailboxListQuotas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/quotas/changes\n  method: get\n  operationId: mailboxGetQuotaChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/sender-choices\n  method:\
  \ get\n  operationId: mailboxGetSenderChoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.send\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/session\n  method: get\n  operationId: mailboxGetSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/submissions\n  method: get\n  operationId: mailboxListSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/submissions/{submission_id}\n  method: get\n  operationId: mailboxGetSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /mailbox/submissions/changes\n  method: get\n  operationId: mailboxGetSubmissionChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/threads\n  method: get\n  operationId: mailboxListThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/threads/{thread_id}\n  method: get\n  operationId: mailboxGetThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/threads/{thread_id}/content\n  method: get\n  operationId: mailboxGetThreadContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/threads/{thread_id}/messages\n  method: get\n  operationId: mailboxListThreadMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/usage\n  method: get\n  operationId: mailboxListUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailboxes\n  method: get\n  operationId: managementListMailboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.admin.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailboxes\n  method: post\n  operationId: managementCreateMailbox\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    scope:\n    - mailbox.admin.create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}\n  method: delete\n  operationId: managementDeleteMailbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.admin.delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}\n  method: get\n  operationId: managementGetMailbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.admin.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailboxes/{public_id}\n  method: patch\n  operationId:\
  \ managementUpdateMailbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}/filters\n  method: get\n  operationId: managementGetMailboxFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.admin.manage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailboxes/{public_id}/filters\n  method: put\n  operationId: managementSetMailboxFilters\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}/keys\n  method: post\n  operationId: managementCreateMailboxKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}/keys/{key_id}\n  method: delete\n  operationId: managementDeleteMailboxKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mailboxes/{public_id}/resume\n\
  \  method: post\n  operationId: managementResumeMailbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}/suspend\n  method: post\n  operationId: managementSuspendMailbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mailbox.admin.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes/{public_id}/usage\n  method: get\n  operationId: managementGetMailboxCostUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    -\
  \ mailbox.admin.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailboxes/availability\n  method: get\n  operationId: managementCheckMailboxAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mailbox.admin.create\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: managementGetConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  operationId: managementListProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - provider.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: post\n  operationId: managementCreateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - provider.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/{public_id}\n  method: delete\n  operationId: managementDeleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - provider.delete\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/{public_id}\n  method: get\n  operationId: managementGetProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - provider.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /providers/{public_id}\n  method: patch\n  operationId: managementUpdateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - provider.update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/{public_id}/activate\n  method: post\n  operationId: managementActivateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - provider.update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (38 KB total) ---\n# Full source: https://artifacts.apis.io/sendmux-ai/agentic-access/sendmux-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/sendmux-ai/agentic-access/sendmux-ai-agentic-access.yml
summary_line: 119 operations · 50 acting · 2 human-in-the-loop
tags:
- Company
- Email
- Artificial Intelligence
- Agents
- Integration
---
