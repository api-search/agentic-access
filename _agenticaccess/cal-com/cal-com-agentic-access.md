---
acting_count: 66
action_class_counts:
  acting: 66
  connected: 55
api_specs:
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Bookings API
  slug: cal-com-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Event Types API
  slug: cal-com-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Schedules API
  slug: cal-com-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Availability API
  slug: cal-com-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Slots API
  slug: cal-com-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Webhooks API
  slug: cal-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com OAuth & Auth API
  slug: cal-com-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Teams API
  slug: cal-com-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Organizations API
  slug: cal-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Out-of-Office API
  slug: cal-com-ooo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Conferencing API
  slug: cal-com-conferencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Destination Calendars API
  slug: cal-com-destination-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Atoms (Platform)
  slug: cal-com-atoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
consequence_counts:
  read: 55
  safety-critical: 66
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 66
kind: agentic-access
layout: agentic-access
method: generated
name: Cal Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/api-keys/refresh
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/auth/oauth2/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/attendees
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/bookings/{bookingUid}/attendees/{attendeeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/confirm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/decline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/guests
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/bookings/{bookingUid}/location
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/mark-absent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/reassign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/reassign/{userId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bookings/{bookingUid}/reschedule
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/calendars/connections/{connectionId}/events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/calendars/connections/{connectionId}/events/{eventId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/calendars/connections/{connectionId}/events/{eventId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/calendars/ics-feed/save
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/calendars/{calendar}/credentials
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/calendars/{calendar}/disconnect
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/calendars/{calendar}/event/{eventUid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/calendars/{calendar}/events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/calendars/{calendar}/events/{eventUid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/calendars/{calendar}/events/{eventUid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/conferencing/{app}/connect
operation_count: 121
overview: 'Cal.com exposes 121 API operations that an AI agent could call, of which 66 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 55 read and 66 safety-critical.


  66 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cal.com
provider_slug: cal-com
slug: cal-com-agentic-access
source_filename: cal-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cal-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 121\n  by_action_class:\n    acting: 66\n    connected: 55\n  by_consequence:\n    safety-critical: 66\n    read: 55\n  human_in_the_loop_required: 66\noperations:\n- path: /v2/api-keys/refresh\n  method: post\n  operationId: ApiKeysController_refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings\n  method: post\n  operationId: BookingsController_2024_08_13_createBooking\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings\n  method: get\n  operationId: BookingsController_2024_08_13_getBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/by-seat/{seatUid}\n  method: get\n  operationId: BookingsController_2024_08_13_getBookingBySeatUid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}\n  method: get\n  operationId: BookingsController_2024_08_13_getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/recordings\n  method: get\n  operationId: BookingsController_2024_08_13_getBookingRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/transcripts\n  method: get\n  operationId: BookingsController_2024_08_13_getBookingTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/reschedule\n  method: post\n  operationId: BookingsController_2024_08_13_rescheduleBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/cancel\n  method: post\n  operationId: BookingsController_2024_08_13_cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/mark-absent\n  method: post\n  operationId: BookingsController_2024_08_13_markNoShow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/reassign\n  method: post\n  operationId: BookingsController_2024_08_13_reassignBooking\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/reassign/{userId}\n  method: post\n  operationId: BookingsController_2024_08_13_reassignBookingToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/confirm\n  method: post\n  operationId: BookingsController_2024_08_13_confirmBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/decline\n  method: post\n  operationId: BookingsController_2024_08_13_declineBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/calendar-links\n  method: get\n  operationId: BookingsController_2024_08_13_getCalendarLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/references\n  method: get\n  operationId: BookingsController_2024_08_13_getBookingReferences\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/conferencing-sessions\n  method: get\n  operationId: BookingsController_2024_08_13_getVideoSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/location\n  method: patch\n  operationId: BookingLocationController_2024_08_13_updateBookingLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/attendees\n  method: get\n  operationId: BookingAttendeesController_2024_08_13_getBookingAttendees\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/attendees\n  method: post\n  operationId: BookingAttendeesController_2024_08_13_addAttendee\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/attendees/{attendeeId}\n  method: get\n  operationId: BookingAttendeesController_2024_08_13_getBookingAttendee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingUid}/attendees/{attendeeId}\n  method: delete\n  operationId: BookingAttendeesController_2024_08_13_removeAttendee\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bookings/{bookingUid}/guests\n  method: post\n  operationId: BookingGuestsController_2024_08_13_addGuests\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/connections\n  method: get\n  operationId: CalUnifiedCalendarsController_listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/calendars/connections/{connectionId}/events\n  method: get\n  operationId: CalUnifiedCalendarsController_listConnectionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/connections/{connectionId}/events\n  method: post\n  operationId: CalUnifiedCalendarsController_createConnectionEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/connections/{connectionId}/events/{eventId}\n  method: get\n  operationId: CalUnifiedCalendarsController_getConnectionEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/connections/{connectionId}/events/{eventId}\n  method: patch\n  operationId: CalUnifiedCalendarsController_updateConnectionEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/connections/{connectionId}/events/{eventId}\n  method: delete\n  operationId: CalUnifiedCalendarsController_deleteConnectionEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/connections/{connectionId}/freebusy\n\
  \  method: get\n  operationId: CalUnifiedCalendarsController_getConnectionFreeBusy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/events/{eventUid}\n  method: get\n  operationId: CalUnifiedCalendarsController_getCalendarEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/events/{eventUid}\n  method: patch\n  operationId: CalUnifiedCalendarsController_updateCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/{calendar}/events/{eventUid}\n\
  \  method: delete\n  operationId: CalUnifiedCalendarsController_deleteCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/{calendar}/event/{eventUid}\n  method: get\n  operationId: CalUnifiedCalendarsController_getCalendarEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/event/{eventUid}\n  method: patch\n  operationId: CalUnifiedCalendarsController_updateCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/{calendar}/events\n  method: get\n  operationId: CalUnifiedCalendarsController_listCalendarEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/events\n  method: post\n  operationId: CalUnifiedCalendarsController_createCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/{calendar}/freebusy\n  method: get\n  operationId: CalUnifiedCalendarsController_getFreeBusy\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/ics-feed/save\n  method: post\n  operationId: CalendarsController_createIcsFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/ics-feed/check\n  method: get\n  operationId: CalendarsController_checkIcsFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/busy-times\n  method: get\n  operationId: CalendarsController_getBusyTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars\n\
  \  method: get\n  operationId: CalendarsController_getCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/connect\n  method: get\n  operationId: CalendarsController_redirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/save\n  method: get\n  operationId: CalendarsController_save\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/credentials\n  method: post\n  operationId: CalendarsController_syncCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/calendars/{calendar}/check\n  method: get\n  operationId: CalendarsController_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/calendars/{calendar}/disconnect\n  method: post\n  operationId: CalendarsController_deleteCalendarCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/conferencing/{app}/connect\n  method: post\n  operationId: ConferencingController_connect\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/conferencing/{app}/oauth/auth-url\n  method: get\n  operationId: ConferencingController_redirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferencing/{app}/oauth/callback\n  method: get\n  operationId: ConferencingController_save\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferencing\n  method: get\n  operationId: ConferencingController_listInstalledConferencingApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferencing/{app}/default\n\
  \  method: post\n  operationId: ConferencingController_default\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/conferencing/default\n  method: get\n  operationId: ConferencingController_getDefault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferencing/{app}/disconnect\n  method: delete\n  operationId: ConferencingController_disconnect\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/users\n  method: get\n  operationId: OAuthClientUsersController_getManagedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/oauth-clients/{clientId}/users\n  method: post\n  operationId: OAuthClientUsersController_createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/users/{userId}\n  method: get\n  operationId: OAuthClientUsersController_getUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/oauth-clients/{clientId}/users/{userId}\n  method: patch\n  operationId: OAuthClientUsersController_updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/users/{userId}\n  method: delete\n  operationId: OAuthClientUsersController_deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/users/{userId}/force-refresh\n  method: post\n  operationId: OAuthClientUsersController_forceRefresh\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth/{clientId}/refresh\n  method: post\n  operationId: OAuthFlowController_refreshTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/webhooks\n  method: post\n  operationId: OAuthClientWebhooksController_createOAuthClientWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/webhooks\n  method: get\n  operationId: OAuthClientWebhooksController_getOAuthClientWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/oauth-clients/{clientId}/webhooks\n  method: delete\n  operationId: OAuthClientWebhooksController_deleteAllOAuthClientWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/webhooks/{webhookId}\n  method: patch\n  operationId:\
  \ OAuthClientWebhooksController_updateOAuthClientWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}/webhooks/{webhookId}\n  method: get\n  operationId: OAuthClientWebhooksController_getOAuthClientWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/oauth-clients/{clientId}/webhooks/{webhookId}\n  method: delete\n  operationId: OAuthClientWebhooksController_deleteOAuthClientWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients\n  method: post\n  operationId: OAuthClientsController_createOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients\n  method: get\n  operationId: OAuthClientsController_getOAuthClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/oauth-clients/{clientId}\n  method: get\n  operationId: OAuthClientsController_getOAuthClientById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/oauth-clients/{clientId}\n  method: patch\n  operationId: OAuthClientsController_updateOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/oauth-clients/{clientId}\n  method: delete\n  operationId: OAuthClientsController_deleteOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/destination-calendars\n  method: put\n  operationId: DestinationCalendarsController_updateDestinationCalendars\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types\n  method: post\n  operationId: EventTypesController_2024_06_14_createEventType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types\n  method: get\n  operationId: EventTypesController_2024_06_14_getEventTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/event-types/{eventTypeId}\n\
  \  method: get\n  operationId: EventTypesController_2024_06_14_getEventTypeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/event-types/{eventTypeId}\n  method: patch\n  operationId: EventTypesController_2024_06_14_updateEventType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}\n  method: delete\n  operationId: EventTypesController_2024_06_14_deleteEventType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/webhooks\n  method: post\n  operationId: EventTypeWebhooksController_createEventTypeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/webhooks\n  method: get\n  operationId: EventTypeWebhooksController_getEventTypeWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/event-types/{eventTypeId}/webhooks\n  method: delete\n  operationId: EventTypeWebhooksController_deleteAllEventTypeWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/webhooks/{webhookId}\n  method: patch\n  operationId: EventTypeWebhooksController_updateEventTypeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/webhooks/{webhookId}\n  method: get\n  operationId: EventTypeWebhooksController_getEventTypeWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/event-types/{eventTypeId}/webhooks/{webhookId}\n  method: delete\n  operationId: EventTypeWebhooksController_deleteEventTypeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/private-links\n  method: post\n  operationId: EventTypesPrivateLinksController_createPrivateLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/private-links\n  method: get\n  operationId: EventTypesPrivateLinksController_getPrivateLinks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/event-types/{eventTypeId}/private-links/{linkId}\n  method: patch\n  operationId: EventTypesPrivateLinksController_updatePrivateLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/event-types/{eventTypeId}/private-links/{linkId}\n  method: delete\n  operationId: EventTypesPrivateLinksController_deletePrivateLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v2/me\n  method: get\n  operationId: MeController_getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/me\n  method: patch\n  operationId: MeController_updateMe\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/auth/oauth2/clients/{clientId}\n  method: get\n  operationId: OAuth2Controller_getClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/oauth2/token\n  method: post\n  operationId: OAuth2Controller_token\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/schedules\n  method: post\n  operationId: SchedulesController_2024_06_11_createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escal\n\n# --- truncated at 32 KB (41 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/agentic-access/cal-com-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/agentic-access/cal-com-agentic-access.yml
summary_line: 121 operations · 66 acting · 66 human-in-the-loop
tags:
- Productivity
- Scheduling
- Calendar
- Open Source
- Booking
---
