---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: rhel-advisories-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux Advisories API
  slug: rhel-advisories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-advisories-api-openapi.yml
- filename: rhel-cves-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux CVEs API
  slug: rhel-cves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-cves-api-openapi.yml
- filename: rhel-oval-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux OVAL API
  slug: rhel-oval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-oval-api-openapi.yml
- filename: rhel-subscriptions-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux Subscriptions API
  slug: rhel-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-subscriptions-api-openapi.yml
- filename: rhel-systems-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux Systems API
  slug: rhel-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-systems-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rhel Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Red Hat Enterprise Linux exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Red Hat Enterprise Linux
provider_slug: rhel
slug: rhel-agentic-access
source_filename: rhel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/rhel-security-data-openapi.yml, openapi/rhel-subscription-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /cve.json\n  method: get\n  operationId: listCVEs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cveId}.json\n  method: get\n  operationId: getCVE\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/{advisoryId}.json\n\
  \  method: get\n  operationId: getAdvisory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oval/com.redhat.rhsa-RHEL{majorVersion}.xml.bz2\n  method: get\n  operationId: getOVALStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems\n  method: get\n  operationId: listSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{uuid}\n  method: get\n  operationId: getSystem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allocations\n  method: get\n  operationId: listAllocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/agentic-access/rhel-agentic-access.yml
summary_line: 8 operations
tags:
- Automation
- Compliance
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
- Security
- Subscription Management
- Vulnerability Management
---
