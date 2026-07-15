---
acting_count: 46
action_class_counts:
  acting: 46
  connected: 27
api_specs:
- filename: momence-openapi.yml
  format: yaml
  label: Momence Authentication API
  slug: momence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Members API
  slug: momence-host-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Sessions & Bookings API
  slug: momence-host-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Memberships API
  slug: momence-host-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Checkout & Sales API
  slug: momence-host-checkout-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Member Account API
  slug: momence-member-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Member Booking API
  slug: momence-member-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
consequence_counts:
  read: 27
  safety-critical: 46
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 46
kind: agentic-access
layout: agentic-access
method: generated
name: Momence Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/auth/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/checkout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/checkout/compatible-memberships
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/checkout/prices
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/members
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/members/list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/credits
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-freeze
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-freeze
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-freeze
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-unfreeze
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-unfreeze
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/name
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/host/members/{memberId}/phone-number
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/members/{memberId}/phone-number
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/members/{memberId}/tags/{tagId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/members/{memberId}/tags/{tagId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/reports
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/session-bookings/{bookingId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/session-bookings/{bookingId}/check-in
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/session-bookings/{bookingId}/check-in
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/host/session-recurring-bookings/{bookingId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/host/sessions/{sessionId}/bookings/free
operation_count: 73
overview: 'Momence exposes 73 API operations that an AI agent could call, of which 46 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 46 safety-critical.


  46 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Momence
provider_slug: momence
slug: momence-agentic-access
source_filename: momence-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/momence-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 73\n  by_action_class:\n    connected: 27\n    acting: 46\n  by_consequence:\n    read: 27\n    safety-critical: 46\n  human_in_the_loop_required: 46\noperations:\n- path: /api/v2/auth/authorize\n  method: get\n  operationId: ApiV2AuthController_authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/auth/token\n  method: post\n  operationId: ApiV2AuthController_token\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/auth/profile\n  method: get\n  operationId: ApiV2AuthController_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/auth/logout\n  method: post\n  operationId: ApiV2AuthController_logout\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/appointments/reservations\n  method: get\n  operationId: ApiV2HostAppointmentsController_getHostAppointmentReservations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/checkout/compatible-memberships\n  method: post\n  operationId: ApiV2HostCheckoutController_postCompatibleMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/checkout/prices\n  method: post\n  operationId: ApiV2HostCheckoutController_postPrices\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/checkout\n\
  \  method: post\n  operationId: ApiV2HostCheckoutController_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/appointments\n  method: get\n  operationId: ApiV2HostMembersAppointmentsController_getAppointmentReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members/{memberId}/bought-memberships/active\n  method: get\n  operationId: ApiV2HostMembersBoughtMembershipsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/credits\n\
  \  method: put\n  operationId: ApiV2HostMembersBoughtMembershipsController_updateClassCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-freeze\n  method: put\n  operationId: ApiV2HostMembersBoughtMembershipsController_freezeMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-freeze\n\
  \  method: put\n  operationId: ApiV2HostMembersBoughtMembershipsController_scheduleMembershipFreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-freeze\n  method: delete\n  operationId: ApiV2HostMembersBoughtMembershipsController_removeMembershipFreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-unfreeze\n\
  \  method: put\n  operationId: ApiV2HostMembersBoughtMembershipsController_scheduleMembershipUnfreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/bought-memberships/{boughtMembershipId}/membership-schedule-unfreeze\n  method: delete\n  operationId: ApiV2HostMembersBoughtMembershipsController_removeMembershipUnfreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members\n  method: get\n  operationId:\
  \ ApiV2HostMembersController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members\n  method: post\n  operationId: ApiV2HostMembersController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/list\n  method: post\n  operationId: ApiV2HostMembersController_listPost\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/v2/host/members/{memberId}\n  method: get\n  operationId: ApiV2HostMembersController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members/{memberId}/name\n  method: put\n  operationId: ApiV2HostMembersController_updateName\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/phone-number\n  method: put\n  operationId: ApiV2HostMembersController_updatePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/phone-number\n  method: delete\n  operationId: ApiV2HostMembersController_deleteMemberPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/email\n  method: put\n  operationId: ApiV2HostMembersController_updateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n-\
  \ path: /api/v2/host/memberships\n  method: get\n  operationId: ApiV2HostMembershipsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members/{memberId}/notes\n  method: get\n  operationId: ApiV2HostMembersNotesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members/{memberId}/sessions\n  method: get\n  operationId: ApiV2HostMembersSessionBookingsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/members/{memberId}/tags/{tagId}\n  method: post\n  operationId: ApiV2HostMemberTagsController_assign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/members/{memberId}/tags/{tagId}\n  method: delete\n  operationId: ApiV2HostMemberTagsController_unassign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/sales\n  method: get\n  operationId: ApiV2HostSalesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/session-bookings/{bookingId}/check-in\n  method: post\n  operationId: ApiV2HostSessionBookingCheckInController_addSessionBookingCheckIn\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/session-bookings/{bookingId}/check-in\n  method: delete\n  operationId: ApiV2HostSessionBookingCheckInController_removeSessionBookingCheckIn\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/session-bookings/{bookingId}\n  method: delete\n  operationId: ApiV2HostSessionBookingController_cancelSessionBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/session-recurring-bookings/{bookingId}\n  method: delete\n  operationId: ApiV2HostSessionRecurringBookingController_cancelRecurringSessionBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/sessions\n  method: get\n  operationId: ApiV2HostSessionsController_getSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/sessions/{sessionId}\n\
  \  method: get\n  operationId: ApiV2HostSessionsController_getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/sessions/{sessionId}/bookings\n  method: get\n  operationId: ApiV2HostSessionsController_getSessionBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/host/sessions/{sessionId}/bookings/free\n  method: post\n  operationId: ApiV2HostSessionsController_addToSessionForFree\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/sessions/{sessionId}/waitlist/bookings\n\
  \  method: post\n  operationId: ApiV2HostSessionsController_addToWaitlist\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/tags\n  method: get\n  operationId: ApiV2HostTagsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member-addresses\n  method: get\n  operationId: ApiV2MemberAddressesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member-addresses\n  method: post\n  operationId: ApiV2MemberAddressesController_create\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member-addresses/{memberAddressId}\n  method: get\n  operationId: ApiV2MemberAddressesController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member-addresses/{memberAddressId}\n  method: put\n  operationId: ApiV2MemberAddressesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member-addresses/{memberAddressId}\n\
  \  method: delete\n  operationId: ApiV2MemberAddressesController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/bought-memberships/active\n  method: get\n  operationId: ApiV2MemberBoughtMembershipsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/bought-memberships/{boughtMembershipId}/membership-freeze\n  method: put\n  operationId: ApiV2MemberBoughtMembershipsController_freezeMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/bought-memberships/{boughtMembershipId}/membership-schedule-freeze\n  method: put\n  operationId: ApiV2MemberBoughtMembershipsController_scheduleMembershipFreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/bought-memberships/{boughtMembershipId}/membership-schedule-freeze\n  method: delete\n  operationId: ApiV2MemberBoughtMembershipsController_removeMembershipFreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/bought-memberships/{boughtMembershipId}/membership-schedule-unfreeze\n  method: put\n  operationId: ApiV2MemberBoughtMembershipsController_scheduleMembershipUnfreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/bought-memberships/{boughtMembershipId}/membership-schedule-unfreeze\n  method: delete\n  operationId: ApiV2MemberBoughtMembershipsController_removeMembershipUnfreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/checkout/compatible-memberships\n  method: post\n  operationId: ApiV2MemberCheckoutController_postCompatibleMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/checkout/prices\n  method: post\n  operationId: ApiV2MemberCheckoutController_postPrices\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/v2/member/checkout\n  method: post\n  operationId: ApiV2MemberCheckoutController_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member\n  method: get\n  operationId: ApiV2MemberController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member\n  method: put\n  operationId: ApiV2MemberController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/visits\n  method: get\n  operationId: ApiV2MemberController_getVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/email\n  method: put\n  operationId: ApiV2MemberController_updateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/phone-number\n  method: put\n  operationId: ApiV2MemberController_updatePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/phone-number\n  method: delete\n  operationId: ApiV2MemberController_deletePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/password-reset-email\n  method: post\n  operationId: ApiV2MemberController_requestPasswordResetEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/host/locations\n\
  \  method: get\n  operationId: ApiV2MemberHostLocationsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/host/memberships\n  method: get\n  operationId: ApiV2MemberHostMembershipsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/host/sessions\n  method: get\n  operationId: ApiV2MemberHostSessionsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/host/signable-documents\n  method: get\n  operationId: ApiV2MemberHostSignableDocumentsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v2/member/host/signable-documents/sign\n  method: put\n  operationId: ApiV2MemberHostSignableDocumentsController_sign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/saved-payment-methods\n  method: get\n  operationId: ApiV2MemberSavedPaymentMethodsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/saved-payment-methods\n  method: post\n  operationId: ApiV2MemberSavedPaymentMethodsController_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n     \
  \ exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/saved-payment-methods/{savedPaymentMethodId}\n  method: delete\n  operationId: ApiV2MemberSavedPaymentMethodsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/member/sessions\n  method: get\n  operationId: ApiV2MemberSessionBookingsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/member/sessions/{sessionBookingId}\n  method: delete\n  operationId: ApiV2MemberSessionBookingsController_cancel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/reports\n  method: post\n  operationId: ApiV2HostReportRunsController_createReportRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/host/reports/{reportRunId}\n  method: get\n  operationId: ApiV2HostReportRunsController_getReportRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/agentic-access/momence-agentic-access.yml
summary_line: 73 operations · 46 acting · 46 human-in-the-loop
tags:
- Fitness
- Wellness
- Studio Management
- Booking
- Scheduling
- Memberships
- Payments
- Class Management
---
