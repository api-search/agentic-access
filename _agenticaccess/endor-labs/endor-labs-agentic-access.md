---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 11
api_specs:
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Projects API
  slug: endor-labs-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Dependencies & Packages API
  slug: endor-labs-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Findings API
  slug: endor-labs-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Policies API
  slug: endor-labs-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Scan Results API
  slug: endor-labs-scan-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Auth & Namespaces API
  slug: endor-labs-auth-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
consequence_counts:
  read: 11
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Endor Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Endor Labs exposes 16 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Endor Labs
provider_slug: endor-labs
slug: endor-labs-agentic-access
source_filename: endor-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/endor-labs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 5\n    connected: 11\n  by_consequence:\n    write: 5\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/api-key\n  method: post\n  operationId: exchangeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/projects/{uuid}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/package-versions\n  method: get\n  operationId: listPackageVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/package-versions/{uuid}\n\
  \  method: get\n  operationId: getPackageVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/findings\n  method: get\n  operationId: listFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/findings/{uuid}\n  method: get\n  operationId: getFinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/policies\n  method: post\n  operationId: createPolicy\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/policies/{uuid}\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/policies/{uuid}\n  method: patch\n  operationId: updatePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/policies/{uuid}\n  method: delete\n  operationId: deletePolicy\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/scan-results\n  method: get\n  operationId: listScanResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/scan-results/{uuid}\n  method: get\n  operationId: getScanResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/agentic-access/endor-labs-agentic-access.yml
summary_line: 16 operations · 5 acting
tags:
- Security
- Software Supply Chain
- SCA
- Reachability
- AppSec
- AI Security
---
