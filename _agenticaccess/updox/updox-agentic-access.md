---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: updox-openapi.yml
  format: yaml
  label: Updox Address Book API
  slug: updox-address-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/openapi/updox-openapi.yml
- filename: updox-openapi.yml
  format: yaml
  label: Updox Faxing API
  slug: updox-faxing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/openapi/updox-openapi.yml
- filename: updox-openapi.yml
  format: yaml
  label: Updox Video Chat API
  slug: updox-video-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/openapi/updox-openapi.yml
consequence_counts:
  physical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Updox Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /VideoCallActions
operation_count: 10
overview: 'Updox exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Updox
provider_slug: updox
slug: updox-agentic-access
source_filename: updox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/updox-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    write: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /Ping\n  method: post\n  operationId: ping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PingWithApplicationAuth\n  method: post\n  operationId: pingWithApplicationAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PingWithAccountAuth\n  method: post\n  operationId: pingWithAccountAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PingWithAuth\n  method: post\n  operationId: pingWithAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressBookList\n  method: post\n  operationId: addressBookList\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressBookSearch\n  method: post\n  operationId: addressBookSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ContactCreate\n  method: post\n  operationId: contactCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /FaxOemPop\n  method: post\n  operationId:\
  \ faxOemPop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PopPDF\n  method: post\n  operationId: popPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /VideoCallActions\n  method: post\n  operationId: videoCallActions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/updox/refs/heads/main/agentic-access/updox-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Healthcare
- Patient Engagement
- Secure Messaging
- Electronic Fax
- Telehealth
- Document Management
- HIPAA
- EverCommerce
---
