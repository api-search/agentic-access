---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: dns-openapi.yml
  format: yaml
  label: Google Cloud DNS API
  slug: google-cloud-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/openapi/dns-openapi.yml
consequence_counts:
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Dns Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Google Cloud DNS exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud DNS
provider_slug: google-cloud-dns
slug: google-cloud-dns-agentic-access
source_filename: google-cloud-dns-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dns-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 5\n    acting: 5\n  by_consequence:\n    read: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/managedZones\n  method: get\n  operationId: listManagedZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones\n  method: post\n  operationId: createManagedZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}\n  method: get\n  operationId: getManagedZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}\n  method: patch\n  operationId: patchManagedZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n  \
  \  - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}\n  method: delete\n  operationId: deleteManagedZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}/rrsets\n  method: get\n  operationId: listResourceRecordSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}/rrsets\n  method: post\n  operationId: createResourceRecordSet\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}/changes\n  method: get\n  operationId: listChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/managedZones/{managedZone}/changes\n  method: post\n  operationId: createChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n- path: /projects/{project}/policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/ndev.clouddns.readwrite\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/agentic-access/google-cloud-dns-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- DNS
- Domain Names
- Google Cloud
- Name Resolution
- Networking
---
