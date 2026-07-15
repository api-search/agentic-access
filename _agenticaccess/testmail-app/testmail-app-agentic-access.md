---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: testmail-app-json-api-openapi.yml
  format: yaml
  label: Testmail JSON API
  slug: testmail-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/openapi/testmail-app-json-api-openapi.yml
- filename: testmail-app-graphql-api-openapi.yml
  format: yaml
  label: Testmail GraphQL API
  slug: testmail-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/openapi/testmail-app-graphql-api-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Testmail App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Testmail exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Testmail
provider_slug: testmail-app
slug: testmail-app-agentic-access
source_filename: testmail-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/testmail-app-graphql-api-openapi.yml, openapi/testmail-app-json-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    write: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /graphql\n  method: post\n  operationId: graphqlQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /json\n  method: get\n  operationId: getEmails\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/agentic-access/testmail-app-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Email Testing
- Developer Tools
- API Testing
- GraphQL
- REST API
- CI/CD
- QA Automation
- Programmable Inboxes
---
