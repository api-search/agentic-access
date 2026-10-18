---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 20
api_specs:
- filename: znanylekarz-addresses-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Addresses API
  slug: znanylekarz-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-addresses-api-openapi.yml
- filename: znanylekarz-api-notification-callbacks-api-openapi.yml
  format: yaml
  label: ZnanyLekarz API Notification Callbacks API
  slug: znanylekarz-api-notification-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-api-notification-callbacks-api-openapi.yml
- filename: znanylekarz-bookings-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Bookings API
  slug: znanylekarz-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-bookings-api-openapi.yml
- filename: znanylekarz-calendar-breaks-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Calendar Breaks API
  slug: znanylekarz-calendar-breaks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-calendar-breaks-api-openapi.yml
- filename: znanylekarz-calendars-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Calendars API
  slug: znanylekarz-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-calendars-api-openapi.yml
- filename: znanylekarz-doctors-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Doctors API
  slug: znanylekarz-doctors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-doctors-api-openapi.yml
- filename: znanylekarz-facilities-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Facilities API
  slug: znanylekarz-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-facilities-api-openapi.yml
- filename: znanylekarz-insurances-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Insurances API
  slug: znanylekarz-insurances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-insurances-api-openapi.yml
- filename: znanylekarz-patient-presence-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Patient Presence API
  slug: znanylekarz-patient-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-patient-presence-api-openapi.yml
- filename: znanylekarz-services-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Services API
  slug: znanylekarz-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-services-api-openapi.yml
- filename: znanylekarz-slots-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Slots API
  slug: znanylekarz-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-slots-api-openapi.yml
consequence_counts:
  read: 20
  safety-critical: 2
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Znanylekarz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/calendar/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /facilities/{facility_id}/doctors/{doctor_id}/opinion-request
operation_count: 44
overview: 'ZnanyLekarz exposes 44 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 22 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ZnanyLekarz
provider_slug: znanylekarz
slug: znanylekarz-agentic-access
source_filename: znanylekarz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/znanylekarz-addresses-api-openapi.yml, openapi/znanylekarz-api-notification-callbacks-api-openapi.yml,\n  openapi/znanylekarz-bookings-api-openapi.yml, openapi/znanylekarz-calendar-breaks-api-openapi.yml,\n  openapi/znanylekarz-calendars-api-openapi.yml, openapi/znanylekarz-doctors-api-openapi.yml,\n  openapi/znanylekarz-facilities-api-openapi.yml, openapi/znanylekarz-insurances-api-openapi.yml,\n  openapi/znanylekarz-patient-presence-api-openapi.yml, openapi/znanylekarz-services-api-openapi.yml,\n  openapi/znanylekarz-slots-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 20\n    acting: 24\n  by_consequence:\n    read: 20\n   \
  \ write: 22\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses\n  method: get\n  operationId: getAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}\n  method: get\n  operationId: getAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}\n  method: patch\n  operationId: updateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/integration\n  method: delete\n  operationId: removeAddressIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /{client-endpoint-url}\n  method: post\n  operationId: PushNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /notifications\n  method: get\n  operationId: PullNotification\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /notifications/multiple\n  method: get\n  operationId: PullMultipleNotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /notifications/release\n  method: post\n  operationId: ReleaseNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings\n  method: get\n  operationId: getBookings\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings/{booking_id}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings/{booking_id}\n  method: delete\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings/{booking_id}/move\n\
  \  method: post\n  operationId: moveBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings/{booking_id}/confirm\n  method: put\n  operationId: confirmBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/opinion-request\n  method: put\n  operationId: requestOpinion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/breaks\n  method: get\n  operationId: getCalendarBreaks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/breaks\n  method: post\n  operationId: addCalendarBreak\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/breaks/{break_id}\n  method: get\n  operationId: getCalendarBreak\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/breaks/{break_id}\n  method: patch\n  operationId: moveCalendarBreak\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/breaks/{break_id}\n  method: delete\n  operationId: deleteCalendarBreak\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/calendar\n  method: get\n  operationId: getCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/calendar/enable\n  method: post\n  operationId: enableCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n\
  - path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/calendar/disable\n  method: post\n  operationId: disableCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors\n  method: get\n  operationId: getDoctors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}\n  method: get\n  operationId: getDoctor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - integration\n- path: /facilities\n  method: get\n  operationId: getFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}\n  method: get\n  operationId: getFacility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /insurance-providers\n  method: get\n  operationId: getInsuranceProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /insurance-providers/{insurance_provider_id}/plans\n  method: get\n  operationId: getInsurancePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/insurance-providers\n  method: get\n  operationId: getAddressInsuranceProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/insurance-providers\n  method: post\n  operationId: addAddressInsuranceProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/insurance-providers\n  method: put\n  operationId: updateOrCreateAddressInsuranceProvider\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/insurance-providers/{insurance_provider_id}\n  method: delete\n  operationId: deleteAddressInsuranceProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings/{booking_id}/presence/patient\n  method: post\n  operationId: markPatientPresence\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/bookings/{booking_id}/presence/patient\n  method: delete\n  operationId: markPatientAbsence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /services\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/services\n\
  \  method: get\n  operationId: getAddressServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/services\n  method: post\n  operationId: addAddressService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/services/{address_service_id}\n  method: get\n  operationId: getAddressService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n\
  - path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/services/{address_service_id}\n  method: patch\n  operationId: updateAddressService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/services/{address_service_id}\n  method: delete\n  operationId: deleteAddressService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/slots\n\
  \  method: get\n  operationId: getSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/slots\n  method: put\n  operationId: replaceSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/slots/{start}/book\n  method: post\n  operationId: bookSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n- path: /facilities/{facility_id}/doctors/{doctor_id}/addresses/{address_id}/slots/{date}\n  method: delete\n  operationId: deleteSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - integration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/agentic-access/znanylekarz-agentic-access.yml
summary_line: 44 operations · 24 acting · 2 human-in-the-loop
tags:
- Company
- Healthcare
- Health Tech
- Appointments
- Booking
- Medical
- Marketplace
- Doctors
- Scheduling
- Poland
- Practice Management
- Telehealth
---
