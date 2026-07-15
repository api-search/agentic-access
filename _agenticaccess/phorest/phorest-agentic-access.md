---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 39
api_specs:
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Clients API
  slug: phorest-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Appointments & Bookings API
  slug: phorest-appointments-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Staff API
  slug: phorest-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Services API
  slug: phorest-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Products & Purchases API
  slug: phorest-products-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Vouchers & Loyalty API
  slug: phorest-vouchers-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Branches API
  slug: phorest-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
- filename: phorest-openapi.yml
  format: yaml
  label: Phorest Reporting & Reviews API
  slug: phorest-reporting-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/openapi/phorest-openapi.yml
consequence_counts:
  physical: 3
  read: 39
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Phorest Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{businessId}/branch/{branchId}/deposit-payment-link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{businessId}/branch/{branchId}/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{businessId}/branch/{branchId}/stock/adjustment
operation_count: 62
overview: 'Phorest exposes 62 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 20 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Phorest
provider_slug: phorest
slug: phorest-agentic-access
source_filename: phorest-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/phorest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 39\n    acting: 23\n  by_consequence:\n    read: 39\n    write: 20\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /{businessId}/client\n  method: get\n  operationId: getClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/client\n  method: post\n  operationId: createClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/client/{clientId}\n  method: get\n  operationId: getClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/client/{clientId}\n  method: put\n  operationId: updateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/client/walkin\n  method: get\n  operationId: getWalkInClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/category/client\n  method: get\n  operationId:\
  \ getClientCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/category/client/{categoryId}\n  method: get\n  operationId: getClientCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/appointment\n  method: get\n  operationId: getAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/appointment/{appointmentId}\n  method: get\n  operationId: getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/appointment/{appointmentId}\n  method:\
  \ put\n  operationId: updateAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/appointment/{appointmentId}/cancel\n  method: post\n  operationId: cancelAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/appointment/{appointmentId}/confirm\n  method: post\n  operationId: confirmAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/appointment/{appointmentId}/checkin\n  method: post\n  operationId: checkInAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/appointments/availability\n  method: post\n  operationId: checkAppointmentAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/booking\n  method: post\n  operationId:\
  \ createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/booking/{bookingId}/cancel\n  method: post\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/booking/{bookingId}/activate\n  method: post\n  operationId: activateBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/booking/{bookingId}/note\n  method: post\n  operationId: appendNoteToBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/deposit-payment-link\n  method: post\n  operationId: createDepositPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/staff\n  method: get\n  operationId:\
  \ getStaffList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/staff/{staffId}\n  method: get\n  operationId: getStaff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/staff-work-time-table\n  method: get\n  operationId: getStaffWorkTimeTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/staff/{staffId}/break\n  method: get\n  operationId: getBreaks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/staff/{staffId}/break\n  method: post\n  operationId:\
  \ createBreak\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/staff/{staffId}/break/{breakId}\n  method: get\n  operationId: getStaffBreak\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/staff/{staffId}/break/{breakId}\n  method: put\n  operationId: updateBreak\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/staff/{staffId}/break/{breakId}\n\
  \  method: delete\n  operationId: deleteBreak\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/service\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/service/{serviceId}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/service-category\n  method: get\n  operationId: getServiceCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/package\n  method: get\n  operationId: getServicePackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/service-special-offer\n  method: get\n  operationId: getServiceSpecialOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/course\n  method: get\n  operationId: getCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/client/{clientId}/course\n  method: get\n  operationId: getClientCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/client/{clientId}/course/{courseId}\n  method: get\n  operationId: getClientCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/client/{clientId}/course/{courseId}\n  method: put\n  operationId: updateClientCourse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch\n  method: get\n  operationId: getBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/worktimetable\n\
  \  method: get\n  operationId: getBranchWorkTimeTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/room\n  method: get\n  operationId: getRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/room/{roomId}\n  method: get\n  operationId: getRoom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/machine\n  method: get\n  operationId: getMachines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/machine/{machineId}\n  method: get\n  operationId:\
  \ getMachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/taxrate\n  method: get\n  operationId: getTaxRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/taxrate/{taxRateId}\n  method: get\n  operationId: getTaxRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/product\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/inventorytransaction\n  method: get\n  operationId: getInventoryTransactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/stock/adjustment\n  method: post\n  operationId: performStockAdjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/purchase\n  method: post\n  operationId: createPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{businessId}/branch/{branchId}/till/{tillId}/balance\n  method: get\n  operationId: getTillBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/salefee\n  method: get\n  operationId: getSaleFeeList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/voucher\n  method: get\n  operationId: getVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/voucher\n  method: post\n  operationId: createVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/voucher/{voucherId}\n  method: get\n  operationId: getVoucher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/voucher/{voucherId}\n  method: put\n  operationId: updateVoucherBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/loyaltypoints\n  method: post\n  operationId: changeLoyaltyPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/csvexportjob\n  method: post\n  operationId: createCsvExportJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{businessId}/branch/{branchId}/csvexportjob/{jobId}\n  method: get\n  operationId: getCsvExportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/review\n  method: get\n  operationId: getReviewList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/review/{reviewId}\n  method:\
  \ get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/leads\n  method: get\n  operationId: getLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/branch/{branchId}/leads/stats\n  method: get\n  operationId: getLeadsStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{businessId}/lead\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phorest/refs/heads/main/agentic-access/phorest-agentic-access.yml
summary_line: 62 operations · 23 acting
tags:
- Salon Software
- Spa Software
- Scheduling
- Point of Sale
- Business Management
- Vertical SaaS
---
