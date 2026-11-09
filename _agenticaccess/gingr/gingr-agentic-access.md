---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 26
api_specs:
- filename: gingr-invoices-api-openapi.yml
  format: yaml
  label: Gingr Invoices API
  slug: gingr-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-invoices-api-openapi.yml
- filename: gingr-payments-api-openapi.yml
  format: yaml
  label: Gingr Payments API
  slug: gingr-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-payments-api-openapi.yml
- filename: gingr-pets-api-openapi.yml
  format: yaml
  label: Gingr Pets API
  slug: gingr-pets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-pets-api-openapi.yml
- filename: gingr-booking-type-rates-api-openapi.yml
  format: yaml
  label: Gingr Booking Type Rates API
  slug: gingr-booking-type-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-booking-type-rates-api-openapi.yml
- filename: gingr-bookings-api-openapi.yml
  format: yaml
  label: Gingr Bookings API
  slug: gingr-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-bookings-api-openapi.yml
- filename: gingr-card-on-file-api-openapi.yml
  format: yaml
  label: Gingr Card On File API
  slug: gingr-card-on-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-card-on-file-api-openapi.yml
- filename: gingr-config-api-openapi.yml
  format: yaml
  label: Gingr Config API
  slug: gingr-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-config-api-openapi.yml
- filename: gingr-group-classes-api-openapi.yml
  format: yaml
  label: Gingr Group Classes API
  slug: gingr-group-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-group-classes-api-openapi.yml
- filename: gingr-parents-api-openapi.yml
  format: yaml
  label: Gingr Parents API
  slug: gingr-parents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-parents-api-openapi.yml
- filename: gingr-payment-api-openapi.yml
  format: yaml
  label: Gingr Payment API
  slug: gingr-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-payment-api-openapi.yml
- filename: gingr-precheck-api-openapi.yml
  format: yaml
  label: Gingr Precheck API
  slug: gingr-precheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-precheck-api-openapi.yml
- filename: gingr-upload-api-openapi.yml
  format: yaml
  label: Gingr Upload API
  slug: gingr-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-upload-api-openapi.yml
consequence_counts:
  physical: 6
  read: 26
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gingr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/bookings/{bookingId}/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices/{invoiceId}/refund-items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/deposits/{depositId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/invoices/{invoiceId}/refund
operation_count: 48
overview: 'Gingr exposes 48 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 16 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gingr
provider_slug: gingr
slug: gingr-agentic-access
source_filename: gingr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gingr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 26\n    acting: 22\n  by_consequence:\n    read: 26\n    write: 16\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/parents\n  method: get\n  operationId: v1ParentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parents\n  method: post\n  operationId: v1ParentsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parents/{parentId}\n  method: get\n  operationId: v1ParentsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parents/{parentId}\n  method: put\n  operationId: v1ParentsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parents/{parentId}\n  method: delete\n  operationId: v1ParentsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/parents/validate-email\n  method: get\n  operationId: v1ParentsValidateEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parents/validate-phone\n  method: get\n  operationId: v1ParentsValidatePhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parents/merge\n  method: post\n  operationId: v1ParentsMerge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pets\n  method: get\n  operationId: v1PetsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pets\n  method: post\n  operationId: v1PetsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pets/{petId}\n  method: get\n  operationId: v1PetsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pets/{petId}\n  method: put\n  operationId: v1PetsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pets/{petId}\n  method: delete\n\
  \  operationId: v1PetsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pets/merge\n  method: post\n  operationId: v1PetsMerge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings\n  method: get\n  operationId: v1BookingsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings\n  method: post\n  operationId: v1BookingsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}\n  method: get\n  operationId: v1BookingsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}\n  method: put\n  operationId: v1BookingsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/cancel\n  method: put\n  operationId: v1BookingsCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/check-in\n  method: post\n  operationId: v1BookingCheckIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/checkout\n  method: post\n  operationId: v1BookingsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/estimate\n\
  \  method: get\n  operationId: v1BookingEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/services\n  method: put\n  operationId: v1BookingAddService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/available-lodgings\n  method: get\n  operationId: v1BookingsAvailableLodgings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/wait-list\n  method: post\n  operationId: v1BookingMoveToWaitList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/accept\n  method: post\n  operationId: v1BookingsAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/service-types\n  method: get\n  operationId: v1ConfigServiceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/service-types/{serviceTypeId}\n  method: get\n  operationId: v1ConfigServiceTypeDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/config/booking-types\n  method: get\n  operationId: v1ConfigBookingTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/lodgings\n  method: get\n  operationId: v1ConfigLodgings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/locations\n  method: get\n  operationId: v1ConfigLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/locations/{locationId}\n  method: get\n  operationId: v1ConfigLocationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices\n  method: get\n\
  \  operationId: v1InvoicesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{invoiceId}\n  method: get\n  operationId: v1InvoiceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/charges\n  method: get\n  operationId: v1InvoicesCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{invoiceId}/refund-items\n  method: post\n  operationId: v1InvoicesRefundItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/charge\n  method: post\n  operationId: v1PaymentsCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/invoices/{invoiceId}\n  method: post\n  operationId: v1PaymentsPayInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/invoices/{invoiceId}/refund\n  method: post\n  operationId: v1PaymentsRefundInvoice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/deposits/{depositId}\n  method: post\n  operationId: v1PaymentsPayDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pets/{petId}/immunizations\n  method: get\n  operationId: v1PetsImmunizationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/pets/{petId}/immunizations/{immunizationTypeId}\n  method: put\n  operationId: v1PetsImmunizationsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pets/immunization/expired\n  method: get\n  operationId: v1PetsImmunizationExpired\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/immunization-types\n  method: get\n  operationId: v1ConfigImmunizationTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pets/{petId}/report-cards\n  method: get\n  operationId: v1PetsReportCardsList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pets/{petId}/report-cards/{reportCardId}\n  method: get\n  operationId: v1ReportCardDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pets/report-card-media\n  method: get\n  operationId: v1ReportCardMediaList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/report-card-form\n  method: get\n  operationId: v1ConfigReportCardForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/gingr/agentic-access/gingr-agentic-access.yml
summary_line: 48 operations · 22 acting
tags:
- Pet Care
- Pet Daycare
- Boarding
- Grooming
- Vertical SaaS
- Scheduling
- Payments
---
