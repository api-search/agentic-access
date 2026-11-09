---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: rdapapi-io-asn-api-openapi.yml
  format: yaml
  label: rdapapi-io ASN API
  slug: rdapapi-io-asn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-asn-api-openapi.yml
- filename: rdapapi-io-domain-api-openapi.yml
  format: yaml
  label: rdapapi-io Domain API
  slug: rdapapi-io-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-domain-api-openapi.yml
- filename: rdapapi-io-entity-api-openapi.yml
  format: yaml
  label: rdapapi-io Entity API
  slug: rdapapi-io-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-entity-api-openapi.yml
- filename: rdapapi-io-health-api-openapi.yml
  format: yaml
  label: rdapapi-io Health API
  slug: rdapapi-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-health-api-openapi.yml
- filename: rdapapi-io-ip-api-openapi.yml
  format: yaml
  label: rdapapi-io IP API
  slug: rdapapi-io-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-ip-api-openapi.yml
- filename: rdapapi-io-nameserver-api-openapi.yml
  format: yaml
  label: rdapapi-io Nameserver API
  slug: rdapapi-io-nameserver-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-nameserver-api-openapi.yml
- filename: rdapapi-io-tlds-api-openapi.yml
  format: yaml
  label: rdapapi-io TLDs API
  slug: rdapapi-io-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rdapapi-io/openapi/rdapapi-io-tlds-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rdapapi Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'rdapapi-io exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: rdapapi-io
provider_slug: rdapapi-io
slug: rdapapi-io-agentic-access
source_filename: rdapapi-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/rdapapi-io-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /domain/{domain}\n  method: get\n  operationId: lookupDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/bulk\n  method: post\n  operationId: bulkDomainLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip/{ip}\n  method: get\n  operationId: lookupIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asn/{asn}\n  method: get\n  operationId: lookupAsn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nameserver/{host}\n  method: get\n  operationId: lookupNameserver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity/{handle}\n  method: get\n  operationId: lookupEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tlds\n  method: get\n  operationId: listTlds\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tlds/{tld}\n  method: get\n  operationId: getTld\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/rdapapi-io/agentic-access/rdapapi-io-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Company
- RDAP
- Domain
- WHOIS
---
