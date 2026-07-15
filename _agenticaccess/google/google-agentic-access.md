---
acting_count: 139
action_class_counts:
  acting: 139
  connected: 82
api_specs:
- filename: books-api-openapi.yml
  format: yaml
  label: Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/books-api-openapi.yml
- filename: google-drive-api-openapi.yml
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-api-openapi.yml
- filename: google-drive-activity-api-openapi.yml
  format: yaml
  label: Google Drive Activity API
  slug: google-drive-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-activity-api-openapi.yml
- filename: google-drive-labels-api-openapi.yml
  format: yaml
  label: Google Drive Labels API
  slug: google-drive-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-labels-api-openapi.yml
- filename: google-calendar-api-openapi.yml
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-calendar-api-openapi.yml
- filename: google-gmail-api-openapi.yml
  format: yaml
  label: Google Gmail API
  slug: google-gmail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-gmail-api-openapi.yml
- filename: google-sheets-api-openapi.yml
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-sheets-api-openapi.yml
- filename: google-docs-api-openapi.yml
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-docs-api-openapi.yml
- filename: google-places-api-openapi.yml
  format: yaml
  label: Google Places API
  slug: google-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-places-api-openapi.yml
- filename: google-gemini-api-openapi.yml
  format: yaml
  label: Google Gemini API
  slug: google-gemini-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-gemini-api-openapi.yml
consequence_counts:
  physical: 10
  read: 82
  safety-critical: 10
  write: 119
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Google Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calendars/{calendarId}/acl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calendars/{calendarId}/acl/watch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /calendars/{calendarId}/acl/{ruleId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /calendars/{calendarId}/acl/{ruleId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /calendars/{calendarId}/acl/{ruleId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /channels/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /channels/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gmail/v1/users/{userId}/settings/cse/keypairs/{keyPairId}:disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gmail/v1/users/{userId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/{name}:disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/drafts/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/settings/sendAs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}/smimeInfo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}/smimeInfo/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}/smimeInfo/{id}/setDefault
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/settings/sendAs/{sendAsEmail}/verify
operation_count: 221
overview: 'Google exposes 221 API operations that an AI agent could call, of which 139 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 82 read, 119 write, 10 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google
provider_slug: google
slug: google-agentic-access
source_filename: google-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/books-api-openapi.yml, openapi/google-calendar-api-openapi.yml, openapi/google-docs-api-openapi.yml,\n  openapi/google-drive-activity-api-openapi.yml, openapi/google-drive-api-openapi.yml, openapi/google-drive-labels-api-openapi.yml,\n  openapi/google-gemini-api-openapi.yml, openapi/google-gmail-api-openapi.yml, openapi/google-sheets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 221\n  by_action_class:\n    connected: 82\n    acting: 139\n  by_consequence:\n    read: 82\n    write: 119\n    safety-critical: 10\n    physical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /volumes\n  method: get\n  operationId: listVolumes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volumes/{volumeId}\n  method: get\n  operationId: getVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/bookshelves\n  method: get\n  operationId: listBookshelves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/bookshelves/{shelf}\n  method: get\n  operationId: getBookshelf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/bookshelves/{shelf}/volumes\n  method: get\n  operationId: listBookshelfVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /mylibrary/bookshelves\n  method: get\n  operationId: listMyBookshelves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/books\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mylibrary/bookshelves/{shelf}\n  method: get\n  operationId: getMyBookshelf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/books\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mylibrary/bookshelves/{shelf}/addVolume\n  method: post\n  operationId: addVolumeToBookshelf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/books\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /mylibrary/bookshelves/{shelf}/clearVolumes\n  method: post\n  operationId: clearVolumesFromBookshelf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/books\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mylibrary/bookshelves/{shelf}/moveVolume\n  method: post\n  operationId: moveVolumeInBookshelf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/books\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mylibrary/bookshelves/{shelf}/removeVolume\n  method: post\n  operationId:\
  \ removeVolumeFromBookshelf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/books\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mylibrary/bookshelves/{shelf}/volumes\n  method: get\n  operationId: listMyBookshelfVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/books\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}/acl/{ruleId}\n  method: get\n  operationId: googleGetaccesscontrolrule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}/acl/{ruleId}\n  method: put\n  operationId: googleUpdateaccesscontrolrule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calendars/{calendarId}/acl/{ruleId}\n  method: patch\n  operationId: googlePatchaccesscontrolrule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calendars/{calendarId}/acl/{ruleId}\n  method: delete\n  operationId: googleDeleteaccesscontrolrule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calendars/{calendarId}/acl\n  method: get\n  operationId: googleReturnaccesscontrolrules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}/acl\n  method: post\n  operationId: googleInsertaccesscontrolrule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calendars/{calendarId}/acl/watch\n  method: post\n  operationId: googleWatchaccesscontrolrules\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calendars/{calendarId}/events/{eventId}\n  method: get\n  operationId: googleGetevent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}/events/{eventId}\n  method: put\n  operationId: googleUpdateevent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events/{eventId}\n  method: patch\n  operationId: googlePatchevent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events/{eventId}\n  method: delete\n  operationId: googleDeleteevent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events/{eventId}/instances\n  method: get\n  operationId: googleInsertevent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}/events/{eventId}/move\n  method: post\n  operationId: googleMoveevent\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events\n  method: get\n  operationId: googleReturneventsfromcalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}/events\n  method: post\n  operationId: googleCreateanevent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events/import\n  method: post\n  operationId: googleImportevent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events/quickAdd\n  method: post\n  operationId: googleQuickaddevent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/events/watch\n  method: post\n  operationId: googleWatchevents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}\n\
  \  method: get\n  operationId: googleGetcalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendarId}\n  method: put\n  operationId: googleUpdatecalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}\n  method: patch\n  operationId: googlePatchcalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}\n  method: delete\n  operationId: googleDeletecalendar\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendarId}/clear\n  method: post\n  operationId: googleClearcalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars\n  method: post\n  operationId: googleCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/calendarList/{calendarId}\n\
  \  method: get\n  operationId: googleGetcalendarlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/calendarList/{calendarId}\n  method: put\n  operationId: googleUpdatecalendarlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/calendarList/{calendarId}\n  method: patch\n  operationId: googlePatchcalendarlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/calendarList/{calendarId}\n\
  \  method: delete\n  operationId: googleRemovecalendaronlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/calendarList\n  method: post\n  operationId: googleInsertcalendaronlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/calendarList\n  method: get\n  operationId: googleListcalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/calendarList/watch\n  method: post\n  operationId:\
  \ googleWatchcalendarlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/settings\n  method: get\n  operationId: googleListcalendarsettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/settings/{setting}\n  method: get\n  operationId: googleGetcalendarsettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/settings/watch\n  method: post\n  operationId: googleWatchcalendarsettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/stop\n  method: post\n  operationId: googleStopcalendarchannel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /colors\n  method: get\n  operationId: googleGetcalendarcolors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /freeBusy\n  method: post\n  operationId: googleQueryfreebusy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents\n  method: post\n  operationId: docs.documents.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/documents\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{documentId}\n  method: get\n  operationId: docs.documents.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/documents\n    - https://www.googleapis.com/auth/documents.readonly\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n\
  \    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{documentId}:batchUpdate\n  method: post\n  operationId: docs.documents.batchUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/documents\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/activity:query\n  method: post\n  operationId: googleDriveactivityActivityQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive.activity\n    - https://www.googleapis.com/auth/drive.activity.readonly\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /about\n  method: get\n  operationId: googleDriveAboutGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: get\n  operationId: googleDriveAppsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive.apps.readonly\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /apps/{appId}\n  method: get\n  operationId: googleDriveAppsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.apps.readonly\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changes\n  method: get\n  operationId: googleDriveChangesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n\
  \    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changes/startPageToken\n  method: get\n  operationId: googleDriveChangesGetstartpagetoken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changes/watch\n  method: post\n  operationId: googleDriveChangesWatch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/stop\n  method: post\n  operationId: googleDriveChannelsStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n\
  \    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /drives\n  method: get\n  operationId: googleDriveDrivesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drives\n  method: post\n  operationId: googleDriveDrivesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drives/{driveId}\n  method: get\n  operationId: googleDriveDrivesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drives/{driveId}\n  method: patch\n  operationId: googleDriveDrivesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drives/{driveId}\n  method: delete\n  operationId: googleDriveDrivesDelete\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drives/{driveId}/hide\n  method: post\n  operationId: googleDriveDrivesHide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drives/{driveId}/unhide\n  method: post\n  operationId: googleDriveDrivesUnhide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: googleDriveFilesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: googleDriveFilesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n\
  \    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/generateIds\n  method: get\n  operationId: googleDriveFilesGenerateids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/trash\n  method: delete\n  operationId: googleDriveFilesEmptytrash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /files/{fileId}\n  method: get\n  operationId: googleDriveFilesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n    - https://www.googleapis.com/auth/drive.metadata.readonly\n    - https://www.googleapis.com/auth/drive.photos.readonly\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}\n  method: patch\n  operationId: googleDriveFilesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.metadata\n\
  \    - https://www.googleapis.com/auth/drive.scripts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}\n  method: delete\n  operationId: googleDriveFilesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.appdata\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}/comments\n  method: get\n  operationId: googleDriveCommentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n \
  \   - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}/comments\n  method: post\n  operationId: googleDriveCommentsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}/comments/{commentId}\n  method: get\n  operationId: googleDriveCommentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}/comments/{commentId}\n  method: patch\n  operationId: googleDriveCommentsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}/comments/{commentId}\n  method: delete\n  operationId: googleDriveCommentsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /files/{fileId}/comments/{commentId}/replies\n  method: get\n  operationId: googleDriveRepliesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}/comments/{commentId}/replies\n  method: post\n  operationId: googleDriveRepliesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}/comments/{commentId}/replies/{replyId}\n  method:\
  \ get\n  operationId: googleDriveRepliesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    - https://www.googleapis.com/auth/drive.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}/comments/{commentId}/replies/{replyId}\n  method: patch\n  operationId: googleDriveRepliesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/drive\n    - https://www.googleapis.com/auth/drive.file\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: requ\n\n# --- truncated at 32 KB (78 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/agentic-access/google-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/agentic-access/google-agentic-access.yml
summary_line: 221 operations · 139 acting · 10 human-in-the-loop
tags:
- Advertising
- Cloud
- Developer
- Google
- Platform
- Search
- T1
---
