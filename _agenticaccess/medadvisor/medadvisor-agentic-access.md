---
acting_count: 67
action_class_counts:
  acting: 67
  connected: 45
api_specs:
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - 3rd-Party Integration
  slug: pharmacy-unified-third-party-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Booking Service
  slug: pharmacy-unified-booking-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Refill Order
  slug: pharmacy-unified-refill-order
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Inbox
  slug: pharmacy-unified-inbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Communication
  slug: pharmacy-unified-communication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Head Office
  slug: pharmacy-unified-head-office
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Pharmacy
  slug: pharmacy-unified-pharmacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
consequence_counts:
  physical: 17
  read: 45
  safety-critical: 1
  write: 49
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Medadvisor Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/account/resetpassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/AddNote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/Complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/CompletedOrder/{orderId}/Refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/CompletedOrder/{orderId}/Reminder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/CompletedOrder/{orderId}/ReturnToStock
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/RefillOrder/Delivery/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/LineItem/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/RefillOrder/LineItem/{orderId}/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/RefillOrder/PendingOrder/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/ProcessPIA
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/SendEScript
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/RefillOrder/UpdateLineItemStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/inbox/addscript
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/inbox/sendscheduled
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/pharmacy/SendBroadcastMessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/pharmacy/SendEScriptTokenToMedViewFlow
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/pharmacy/notify
operation_count: 112
overview: 'MedAdvisor exposes 112 API operations that an AI agent could call, of which 67 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 49 write, 17 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MedAdvisor
provider_slug: medadvisor
slug: medadvisor-agentic-access
source_filename: medadvisor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/medadvisor-pharmacy-unified-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 112\n  by_action_class:\n    acting: 67\n    connected: 45\n  by_consequence:\n    write: 49\n    safety-critical: 1\n    read: 45\n    physical: 17\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/account/3rdpartylogin\n  method: post\n  operationId: Account_LoginPharmacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/resetpassword\n\
  \  method: post\n  operationId: Account_ResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/gettime\n  method: get\n  operationId: BookingService_GetPharmacyTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/allservices\n  method: get\n  operationId: BookingService_AllServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/eventresource\n  method: get\n  operationId: BookingService_RetrieveEventResources\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/services/dynamic\n  method: get\n  operationId: BookingService_RetrieveDynamicServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/services/available\n  method: get\n  operationId: BookingService_RetrieveAvailableServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/eventresource/{resourceId}\n  method: get\n  operationId: BookingService_RetrieveEventResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/services/booking/{bookingId}\n\
  \  method: get\n  operationId: BookingService_RetrieveBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/calendartoken/{resetStaffUrl}\n  method: get\n  operationId: BookingService_RetrieveCalendarAccessTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/services/dynamic/{capabilityId}\n  method: get\n  operationId: BookingService_RetrieveDynamicServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/services/available/{capabilityId}\n  method: get\n  operationId: BookingService_RetrieveAvailableServices\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/calendartokendetails/{calendarToken}/{staffToken}\n  method: get\n  operationId: BookingService_RetrieveCalendarTokenDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/retrieveavailabletimeslots\n  method: get\n  operationId: BookingService_RetrieveAvailableTimeslots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/availabletimeslotnewbooking\n  method: get\n  operationId: BookingService_RetrieveAvailableTimeSlotNewBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/pharmacy/retrieveeventbookings\n\
  \  method: get\n  operationId: BookingService_RetrieveEventBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookingservice/patientsearch\n  method: post\n  operationId: BookingService_SearchPatients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/services/update\n  method: post\n  operationId: BookingService_UpdateEventService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/services/historic\n\
  \  method: post\n  operationId: BookingService_RetrieveHistoricBookings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/createeventbooking\n  method: post\n  operationId: BookingService_CreateEventBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/services/suggested\n  method: post\n  operationId: BookingService_RetrieveSuggestedServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/eventbooking/update\n  method: post\n  operationId: BookingService_UpdateEventBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/eventresource/update\n  method: post\n  operationId: BookingService_UpdateEventResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/eventpreferences/update\n  method:\
  \ post\n  operationId: BookingService_UpdateEventPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/services/generate\n  method: post\n  operationId: BookingService_GenerateServiceBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/print/{bookingCode}\n  method: post\n  operationId: BookingService_Print\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/services/bookingedit\n  method: post\n  operationId: BookingService_EditBookingWithCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/eventresource/create/{name}\n  method: post\n  operationId: BookingService_CreateEventResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/services/delete/{serviceId}\n\
  \  method: post\n  operationId: BookingService_DeleteEventService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/eventbooking/{bookingId}/delete\n  method: post\n  operationId: BookingService_DeleteEventBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/eventresource/update/{resourceId}\n  method: post\n  operationId: BookingService_UpdateEventResourceAssociateService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/eventresource/{resourceId}/delete\n  method: post\n  operationId: BookingService_DeleteEventResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/bookingsearch\n  method: post\n  operationId: BookingService_BookingSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/bookingservice/pharmacy/services/availableresource/{capabilityId}\n  method: post\n  operationId: BookingService_RetrieveAvailableResourceForCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/pharmacy/services/deletebooking/{bookingId}\n  method: delete\n  operationId: BookingService_DeleteServiceBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bookingservice/deletebookingrequest/{patientId}/{bookingId}\n  method: delete\n  operationId: BookingService_DeleteBookingRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/comunication/GetPatientGroups\n  method: get\n  operationId: Communication_GetPatientGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comunication/GetAllPatientGroupMembers\n  method: get\n  operationId: Communication_GetAllPatientGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comunication/AddPatientGroup\n  method: post\n  operationId: Communication_AddPatientGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/comunication/EditPatientGroup\n  method: post\n  operationId: Communication_EditPatientGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/comunication/UpdatePatientGroupMembers\n  method: post\n  operationId: Communication_UpdatePatientGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/comunication/DeletePatientGroup/{id}\n\
  \  method: delete\n  operationId: Communication_DeletePatientGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/config/demographicRules\n  method: get\n  operationId: Config_RetrieveDemographicRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/config/precursorInstructions\n  method: get\n  operationId: Config_RetrievePrecursorInstructionMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/drug/escript/{token}\n  method: get\n  operationId: Drug_RetrieveEPrescription3rdParty\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hq/services\n  method: get\n  operationId: HeadOffice_GetServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hq/services\n  method: post\n  operationId: HeadOffice_CreateService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hq/pharmacies\n  method: get\n  operationId: HeadOffice_GetPharmacies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hq/services/{id}\n  method: get\n  operationId: HeadOffice_GetService\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hq/services/{id}\n  method: put\n  operationId: HeadOffice_UpdateService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hq/pharmacies/{id}\n  method: get\n  operationId: HeadOffice_GetPharmacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hq/services/{id}/push/{pharmacyId}/deadline\n  method: put\n  operationId: HeadOffice_UpdatePushDeadline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hq/services/{id}/push\n  method: post\n  operationId: HeadOffice_PushService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/main\n  method: get\n  operationId: Inbox_GetInboxMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inbox/sent\n  method: post\n  operationId: Inbox_GetSentMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/addscript\n  method: post\n  operationId: Inbox_AddScript\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/completed\n  method: post\n  operationId: Inbox_GetCompletedMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/scheduled\n  method: post\n  operationId: Inbox_GetScheduledMessages\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/sendscheduled\n  method: post\n  operationId: Inbox_SendScheduledMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/readytocollect\n  method: post\n  operationId: Inbox_ReadyToCollectMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/dismissmultiple\n  method: post\n  operationId: Inbox_DismissMultiple\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/logging\n  method: post\n  operationId: Logging_Core_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy\n  method: get\n  operationId: Pharmacy_GetPharmacyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/pharmacy/{id}\n  method: get\n  operationId: Pharmacy_PharmacyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/settings\n  method: get\n  operationId: Pharmacy_RetrievePharmacySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/settings\n  method: put\n  operationId: Pharmacy_UpdatePharmacySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/GetAuthInfo\n  method: get\n  operationId: Pharmacy_GetAuthInfo\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/ho-pending-activations\n  method: get\n  operationId: Pharmacy_GetHoPendingActivations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/PharmacyHasPendingHshSms\n  method: get\n  operationId: Pharmacy_PharmacyHasPendingHshSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/GetPharmacyModuleSettings\n  method: get\n  operationId: Pharmacy_GetPharmacyModuleSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/GetPharmacyActivatingBanner\n  method: get\n  operationId: Pharmacy_GetPharmacyActivatingBanner\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/ElectronicPrescribingSettings\n  method: get\n  operationId: Pharmacy_GetPharmacyElectronicPrescribingSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/RetrievePharmaciesWithPendingSMSReminders\n  method: get\n  operationId: Pharmacy_RetrievePharmaciesWithPendingSMSReminders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/PendingHshSmsMessage\n  method: get\n  operationId: Pharmacy_GetPendingHshSmsMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/RetrieveSMSReminderPending\n\
  \  method: get\n  operationId: Pharmacy_RetrieveSMSReminderPending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/RetrievePlusOneQueuedActions\n  method: get\n  operationId: Pharmacy_RetrievePlusOneQueuedActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/GetPharmacyReleaseNotes\n  method: get\n  operationId: Pharmacy_GetPharmacyReleaseNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/GetPharmacyReleaseNotesByType\n  method: get\n  operationId: Pharmacy_GetPharmacyReleaseNotesByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/pharmacy/logo\n  method: get\n  operationId: Pharmacy_GetPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/logo\n  method: post\n  operationId: Pharmacy_UploadLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/GetModuleSettingsByIdentifier\n  method: get\n  operationId: Pharmacy_GetModuleSettingsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/GetPharmacySettingByIdentifier\n  method: get\n  operationId: Pharmacy_GetPharmacySettingByIdentifier\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy/notify\n  method: post\n  operationId: Pharmacy_NotifyPharmacyOfECommerceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/features\n  method: post\n  operationId: Pharmacy_SearchPharmacyFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/SearchPatients\n\
  \  method: post\n  operationId: Pharmacy_SearchPatients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/getpharmacyinfos\n  method: post\n  operationId: Pharmacy_GetPharmacyInfos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/RegisterAccountV4\n  method: post\n  operationId: Pharmacy_RegisterAccountV4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/UpdateActionStatus\n  method: post\n  operationId: Pharmacy_UpdateActionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/UpdateCachePatient\n  method: post\n  operationId: Pharmacy_UpdateCachePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/VerifyPharmacyInfo\n  method: post\n  operationId: Pharmacy_VerifyPharmacyInfo\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/SearchPatientAdvance\n  method: post\n  operationId: Pharmacy_SearchPatientAdvance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/SendBroadcastMessage\n  method: post\n  operationId: Pharmacy_SendBroadcastMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/AcceptTermsConditions\n  method: post\n  operationId: Pharmacy_AcceptTermsConditions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/GenerateActivationCodeV3\n  method: post\n  operationId: Pharmacy_GenerateActivationCodeV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/UpdateSMSReminderComplete\n  method: post\n  operationId: Pharmacy_UpdateSMSReminderComplete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/GeneratePharmacyChangeRequest\n  method: post\n  operationId: Pharmacy_GeneratePharmacyChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pharmacy/SendEScriptTokenToMedViewFlow\n  method: post\n  operationId: Pharmacy_SendEScriptTokenToMedViewFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/RefillOrder/PendingOrder/{orderId}\n  method: get\n  operationId: RefillOrder_GetPendingOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/RefillOrder/PendingOrder/{orderId}\n  method: delete\n  operationId: RefillOrder_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/RefillOrder/CompletedOrder/{\n\n# --- truncated at 32 KB (36 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/agentic-access/medadvisor-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/agentic-access/medadvisor-agentic-access.yml
summary_line: 112 operations · 67 acting · 1 human-in-the-loop
tags:
- Healthcare
- Australia
- Pharmacy
- Medication Management
- Medication Adherence
- e-Prescribing
- eScript
- Patient Engagement
- Appointment Booking
- Digital Health
- Healthcare API
---
