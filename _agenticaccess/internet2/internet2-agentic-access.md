---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 7
api_specs:
- filename: internet2-co-api-openapi.yml
  format: yaml
  label: Internet2 Co API
  slug: internet2-co-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-api-openapi.yml
- filename: internet2-co-group-members-api-openapi.yml
  format: yaml
  label: Internet2 Co Group Members API
  slug: internet2-co-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-group-members-api-openapi.yml
- filename: internet2-co-group-members-json-api-openapi.yml
  format: yaml
  label: Internet2 Co Group Members.json API
  slug: internet2-co-group-members-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-group-members-json-api-openapi.yml
- filename: internet2-co-groups-api-openapi.yml
  format: yaml
  label: Internet2 Co Groups API
  slug: internet2-co-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-groups-api-openapi.yml
- filename: internet2-co-groups-json-api-openapi.yml
  format: yaml
  label: Internet2 Co Groups.json API
  slug: internet2-co-groups-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-groups-json-api-openapi.yml
- filename: internet2-co-people-api-openapi.yml
  format: yaml
  label: Internet2 Co People API
  slug: internet2-co-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-people-api-openapi.yml
- filename: internet2-co-people-json-api-openapi.yml
  format: yaml
  label: Internet2 Co People.json API
  slug: internet2-co-people-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-people-json-api-openapi.yml
- filename: internet2-email-addresses-json-api-openapi.yml
  format: yaml
  label: Internet2 Email Addresses.json API
  slug: internet2-email-addresses-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-email-addresses-json-api-openapi.yml
consequence_counts:
  physical: 3
  read: 7
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Internet2 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /co_group_members/{id}.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /co_groups/reconcile.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /co_groups/reconcile/{id}.json
operation_count: 19
overview: 'Internet2 exposes 19 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 9 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Internet2
provider_slug: internet2
slug: internet2-agentic-access
source_filename: internet2-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/comanage-registry-restapiv1.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 7\n    acting: 12\n  by_consequence:\n    read: 7\n    write: 9\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /co_group_members.json\n  method: get\n  operationId: getCoGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co_group_members.json\n  method: post\n  operationId: addCoGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_group_members/{id}.json\n  method: delete\n  operationId: deleteCoGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_group_members/{id}.json\n  method: get\n  operationId: getCoGroupMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co_group_members/{id}.json\n  method: put\n  operationId: editCoGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n     \
  \ purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_groups/{id}.json\n  method: delete\n  operationId: deleteCoGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_groups/{id}.json\n  method: get\n  operationId: getCoGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co_groups/{id}.json\n  method: put\n  operationId: editCoGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_groups.json\n  method: get\n  operationId: getCoGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co_groups.json\n  method: post\n  operationId: addCoGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_groups/reconcile.json\n  method: put\n  operationId: reconcileAllCoGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /co_groups/reconcile/{id}.json\n  method: post\n  operationId: reconcileCoGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_people.json\n  method: get\n  operationId: getCoPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co_people.json\n  method: post\n  operationId: addCoPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /co_people/{id}.json\n  method: delete\n  operationId: deleteCoPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co_people/{id}.json\n  method: get\n  operationId: getCoPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co_people/{id}.json\n  method: put\n  operationId: editCoPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email_addresses.json\n\
  \  method: get\n  operationId: getEmailAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email_addresses.json\n  method: post\n  operationId: addEmailAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/agentic-access/internet2-agentic-access.yml
summary_line: 19 operations · 12 acting
tags:
- Company
- Networking
- Research
- Education
- Nonprofit
---
