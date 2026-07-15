---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Estimate API
  slug: taskrabbit-home-services-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Availability API
  slug: taskrabbit-home-services-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Booking API
  slug: taskrabbit-home-services-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Catalog API
  slug: taskrabbit-home-services-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Delivery API (Dolly)
  slug: taskrabbit-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
consequence_counts:
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Taskrabbit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'TaskRabbit exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TaskRabbit
provider_slug: taskrabbit
slug: taskrabbit-agentic-access
source_filename: taskrabbit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/taskrabbit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 9\n    connected: 5\n  by_consequence:\n    write: 9\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/estimate\n  method: post\n  operationId: estimateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/availability\n  method: post\n  operationId: checkProjectAvailability\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/bid\n  method: post\n  operationId: bidProjectAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/book\n  method: post\n  operationId: bookProjectAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/list\n  method: post\n  operationId:\
  \ listProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_uuid}\n  method: get\n  operationId: getProjectByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_uuid}/cancel\n  method: post\n  operationId: cancelBookedProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_uuid}/reschedule-availability\n  method: get\n  operationId: getRescheduleAvailability\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_uuid}/reschedule\n  method: post\n  operationId: rescheduleProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_uuid}/services\n  method: get\n  operationId: listServicesByBrandUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_uuid}/external-identifier\n  method: put\n  operationId: updateServiceExternalIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deliveries\n  method: post\n  operationId: createDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: getPartnerInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: pingDeliveryApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/agentic-access/taskrabbit-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Gig Economy
- Handyman
- Home Services
- Marketplace
- Delivery
- Moving
- Partner API
- IKEA
---
