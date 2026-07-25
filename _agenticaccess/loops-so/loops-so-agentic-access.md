---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 14
api_specs:
- filename: loops-so-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-so-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-api-key-api-openapi.yml
- filename: loops-so-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-so-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-campaigns-api-openapi.yml
- filename: loops-so-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-so-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-components-api-openapi.yml
- filename: loops-so-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-so-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-contact-properties-api-openapi.yml
- filename: loops-so-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-so-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-contacts-api-openapi.yml
- filename: loops-so-dedicated-sending-ips-api-openapi.yml
  format: yaml
  label: Loops Dedicated sending IPs API
  slug: loops-so-dedicated-sending-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-dedicated-sending-ips-api-openapi.yml
- filename: loops-so-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-so-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-email-messages-api-openapi.yml
- filename: loops-so-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-so-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-events-api-openapi.yml
- filename: loops-so-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-so-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-mailing-lists-api-openapi.yml
- filename: loops-so-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-so-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-themes-api-openapi.yml
- filename: loops-so-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-so-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-transactional-emails-api-openapi.yml
- filename: loops-so-uploads-api-openapi.yml
  format: yaml
  label: Loops Uploads API
  slug: loops-so-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/openapi/loops-so-uploads-api-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Loops So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactional
operation_count: 26
overview: 'Loops exposes 26 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Loops
provider_slug: loops-so
slug: loops-so-agentic-access
source_filename: loops-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/loops-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 14\n    acting: 12\n  by_consequence:\n    read: 14\n    write: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api-key\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/create\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /contacts/update\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/find\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/delete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/suppression\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/suppression\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/properties\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/properties\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated-sending-ips\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/send\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactional\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /transactional\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /themes/{themeId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /themes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components/{componentId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaignId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaignId}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-messages/{emailMessageId}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-messages/{emailMessageId}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads/{id}/complete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/agentic-access/loops-so-agentic-access.yml
summary_line: 26 operations · 12 acting
tags:
- Email
- Marketing Email
- Transactional Email
- Email Automation
- Email Campaigns
- Email Workflows
- Contacts
- Audience Management
- Events
- Webhooks
- SaaS
- Developer Tools
---
