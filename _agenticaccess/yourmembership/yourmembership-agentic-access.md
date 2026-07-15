---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Members API
  slug: yourmembership-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Events API
  slug: yourmembership-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Certifications API
  slug: yourmembership-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YMCareers API
  slug: yourmembership-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Content and Community API
  slug: yourmembership-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Commerce and Sales API
  slug: yourmembership-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
consequence_counts:
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yourmembership Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'YourMembership exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: YourMembership
provider_slug: yourmembership
slug: yourmembership-agentic-access
source_filename: yourmembership-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/yourmembership-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 2\n    connected: 10\n  by_consequence:\n    write: 2\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /Ams/Authenticate\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Ams/MemberProfile\n  method: get\n  operationId: readContacts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/MemberProfile\n  method: post\n  operationId: upsertMemberProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Ams/People\n  method: get\n  operationId: readContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Events/{eventId}/Registrations\n  method: get\n  operationId: listEventRegistrations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Certifications\n  method: get\n  operationId: listCertifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Community/Messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Community/Groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Store/Orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Store/Orders/{orderId}\n\
  \  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Ams/Exports/Transactions\n  method: get\n  operationId: exportTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/agentic-access/yourmembership-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- Careers
- Community Brands
- Momentive Software
---
