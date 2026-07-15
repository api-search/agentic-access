---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Reports API
  slug: goodhire-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Requestors API
  slug: goodhire-requestors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Packages API
  slug: goodhire-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Webhooks API
  slug: goodhire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Partner API
  slug: goodhire-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Goodhire Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'GoodHire exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoodHire
provider_slug: goodhire
slug: goodhire-agentic-access
source_filename: goodhire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/goodhire-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /company/{company_id}/requestor/{requestor_id}/report/queue\n  method: post\n  operationId: queueReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/{company_id}/requestor/{requestor_id}/report/{report_id}\n  method:\
  \ get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_id}/requestor/{requestor_id}/report\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_id}/requestor/{requestor_id}/productbundles\n  method: get\n  operationId: listProductBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_id}/requestors\n  method: get\n  operationId: listRequestors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_id}/requestors\n  method: post\n  operationId:\
  \ createRequestor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/{company_id}/requestor/{requestor_id}\n  method: get\n  operationId: getRequestor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_id}/requestor/{requestor_id}/partnerappaccess/stepselectreport\n  method: post\n  operationId: partnerSelectReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/agentic-access/goodhire-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Background Checks
- Employment Screening
- Identity Verification
- HR
- Compliance
- FCRA
- Checkr
---
