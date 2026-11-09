---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: crewofthecaptain-com-types-api-openapi.yml
  format: yaml
  label: Crew of the Captain Types API
  slug: crewofthecaptain-com-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crewofthecaptain-com/openapi/crewofthecaptain-com-types-api-openapi.yml
- filename: crewofthecaptain-com-validation-api-openapi.yml
  format: yaml
  label: Crew of the Captain Validation API
  slug: crewofthecaptain-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crewofthecaptain-com/openapi/crewofthecaptain-com-validation-api-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crewofthecaptain Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Crew of the Captain exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crew of the Captain
provider_slug: crewofthecaptain-com
slug: crewofthecaptain-com-agentic-access
source_filename: crewofthecaptain-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crewofthecaptain-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 1\n    acting: 6\n  by_consequence:\n    read: 1\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/validate/iban\n  method: post\n  operationId: validate_iban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate/eu-vat\n  method: post\n  operationId: validate_eu_vat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate/pl-nip\n  method: post\n  operationId: validate_pl_nip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate/pl-regon\n  method: post\n  operationId: validate_pl_regon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate/pl-pesel\n  method: post\n  operationId: validate_pl_pesel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate/email\n  method: post\n  operationId: validate_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/crewofthecaptain-com/agentic-access/crewofthecaptain-com-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Software House
- Web Development
- Marketplace Apps
- Creative Tools
- Automation
---
