---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Access Token API
  slug: vagaro-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Appointments API
  slug: vagaro-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Customers API
  slug: vagaro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Employees API
  slug: vagaro-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Employee Management API
  slug: vagaro-employee-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Locations API
  slug: vagaro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
consequence_counts:
  read: 8
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vagaro Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Vagaro exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vagaro
provider_slug: vagaro
slug: vagaro-agentic-access
source_filename: vagaro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vagaro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 3\n    connected: 8\n  by_consequence:\n    write: 3\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /merchants/generate-access-token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments\n  method: get\n  operationId: listAppointments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{appointmentId}\n  method: get\n  operationId: getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}\n\
  \  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/locations/{businessId}/assignment\n  method: put\n  operationId: assignEmployeeToLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/locations/{businessId}/assignment\n  method: delete\n  operationId: unassignEmployeeFromLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{businessId}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/agentic-access/vagaro-agentic-access.yml
summary_line: 11 operations · 3 acting
tags:
- Salon
- Spa
- Fitness
- Wellness
- Scheduling
- Booking
- Vertical SaaS
---
