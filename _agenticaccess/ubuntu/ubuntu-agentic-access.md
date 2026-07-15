---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 16
api_specs:
- filename: ubuntu-launchpad-openapi.yml
  format: yaml
  label: Launchpad API
  slug: launchpad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-launchpad-openapi.yml
- filename: ubuntu-snap-store-openapi.yml
  format: yaml
  label: Snap Store API
  slug: snap-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-snap-store-openapi.yml
- filename: ubuntu-cve-openapi.yml
  format: yaml
  label: Ubuntu CVE API
  slug: ubuntu-cve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-cve-openapi.yml
consequence_counts:
  read: 16
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ubuntu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Ubuntu exposes 18 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ubuntu
provider_slug: ubuntu
slug: ubuntu-agentic-access
source_filename: ubuntu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ubuntu-cve-openapi.yml, openapi/ubuntu-launchpad-openapi.yml, openapi/ubuntu-snap-store-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 16\n    acting: 2\n  by_consequence:\n    read: 16\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /cves.json\n  method: get\n  operationId: listCves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves/{cve_id}.json\n  method: get\n  operationId: getCve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /notices.json\n  method: get\n  operationId: listNotices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notices/{notice_id}.json\n  method: get\n  operationId: getNotice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /~{person_name}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bugs\n  method: get\n  operationId: listBugs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bugs/{bug_id}\n  method: get\n  operationId: getBug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bugs/{bug_id}\n  method: patch\n  operationId: updateBug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{project_name}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /ubuntu\n  method: get\n  operationId: getUbuntuDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ubuntu/+source/{source_package_name}\n  method: get\n  operationId: getSourcePackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snaps/search\n  method: get\n  operationId: searchSnaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snaps/info/{snap_name}\n  method: get\n  operationId: getSnapInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snaps/refresh\n  method: post\n  operationId:\
  \ refreshSnaps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/snaps/categories\n  method: get\n  operationId: listSnapCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/metrics\n  method: get\n  operationId: getSnapMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/agentic-access/ubuntu-agentic-access.yml
summary_line: 18 operations · 2 acting
tags:
- Cloud
- Containers
- Devops
- Enterprise
- Linux
- Security
- Ubuntu
- Package Management
- Open Source
---
