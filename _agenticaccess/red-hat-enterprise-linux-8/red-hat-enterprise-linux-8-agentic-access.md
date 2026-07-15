---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: openapi.json
  format: json
  label: RHEL 8 Subscription Management API
  slug: subscription-management-api
  spec_type: OpenAPI
  url: https://api.access.redhat.com/management/v1/openapi.json
- filename: openapi.json
  format: json
  label: RHEL 8 Insights API
  slug: insights-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/insights/v1/openapi.json
- filename: openapi.json
  format: json
  label: RHEL 8 Image Builder API
  slug: image-builder-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/image-builder/v1/openapi.json
- filename: openapi.json
  format: json
  label: RHEL 8 Patch Management API
  slug: patch-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/patch/v3/openapi.json
- filename: openapi.json
  format: json
  label: RHEL 8 Vulnerability Management API
  slug: vulnerability-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/vulnerability/v1/openapi.json
- filename: openapi.json
  format: json
  label: RHEL 8 Compliance API
  slug: compliance-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/compliance/v2/openapi.json
- filename: red-hat-enterprise-linux-8-security-data-openapi.yml
  format: yaml
  label: RHEL 8 Security Data API
  slug: security-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-enterprise-linux-8/refs/heads/main/openapi/red-hat-enterprise-linux-8-security-data-openapi.yml
- filename: openapi.json
  format: json
  label: RHEL 8 Host Inventory API
  slug: host-inventory-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/inventory/v1/openapi.json
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Red Hat Enterprise Linux 8 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Red Hat Enterprise Linux 8 exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Red Hat Enterprise Linux 8
provider_slug: red-hat-enterprise-linux-8
slug: red-hat-enterprise-linux-8-agentic-access
source_filename: red-hat-enterprise-linux-8-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/red-hat-enterprise-linux-8-security-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /cve.json\n  method: get\n  operationId: listCves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{CVE}.json\n  method: get\n  operationId: getCve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advisory.json\n  method: get\n  operationId: listAdvisories\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advisory/{advisory}.json\n  method: get\n  operationId: getAdvisory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oval/{product}.xml\n  method: get\n  operationId: getOvalDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-enterprise-linux-8/refs/heads/main/agentic-access/red-hat-enterprise-linux-8-agentic-access.yml
summary_line: 5 operations
tags:
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
---
