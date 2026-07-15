---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 11
api_specs:
- filename: messente-openapi.yml
  format: yaml
  label: Messente Omnimessage API
  slug: messente-omnimessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente SMS API
  slug: messente-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Contacts API
  slug: messente-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Groups API
  slug: messente-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Number Lookup API
  slug: messente-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Statistics API
  slug: messente-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Delivery Reports API
  slug: messente-delivery-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Messente Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /omnimessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /omnimessages
operation_count: 28
overview: 'Messente exposes 28 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 15 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Messente
provider_slug: messente
slug: messente-agentic-access
source_filename: messente-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/messente-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 17\n    connected: 11\n  by_consequence:\n    physical: 2\n    write: 15\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /omnimessage\n  method: post\n  operationId: sendOmnimessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omnimessage/{omnimessageId}\n  method: delete\n\
  \  operationId: cancelScheduledMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omnimessage/{omnimessageId}/status\n  method: get\n  operationId: retrieveDeliveryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /omnimessages\n  method: post\n  operationId: sendBulkOmnimessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/contacts\n \
  \ method: get\n  operationId: fetchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/contacts/{phone}\n  method: get\n  operationId: fetchContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/contacts/{phone}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/contacts/{phone}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/contacts/{phone}/groups\n  method: get\n  operationId: fetchContactGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/groups/{groupId}/contacts/{phone}\n  method: post\n  operationId: addContactToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/groups/{groupId}/contacts/{phone}\n  method: delete\n  operationId: removeContactFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/groups\n  method: get\n  operationId: fetchGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/groups/{groupId}\n  method: get\n  operationId: fetchGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/groups/{groupId}\n  method: put\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/groups/{groupId}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /phonebook/blacklist\n  method: get\n  operationId: fetchBlacklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/blacklist\n  method: post\n  operationId: addToBlacklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebook/blacklist/{phone}\n  method: get\n  operationId: isBlacklisted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebook/blacklist/{phone}\n  method: delete\n  operationId: deleteFromBlacklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hlr/sync\n  method: post\n  operationId: fetchInfoSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/start\n  method: post\n  operationId: verifyNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/pin\n  method: post\n  operationId: verifyPin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statistics/reports\n  method: post\n  operationId: createStatisticsReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricelist\n  method: get\n  operationId: getPricelist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices\n  method: get\n  operationId: getPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_balance\n  method:\
  \ get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/agentic-access/messente-agentic-access.yml
summary_line: 28 operations · 17 acting
tags:
- CPaaS
- Messaging
- SMS
- Viber
- WhatsApp
- Verification
- 2FA
---
