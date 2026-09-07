---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: canonical-snapd-rest-api-openapi.yml
  format: yaml
  label: snapd REST API
  slug: snapd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snapd-rest-api-openapi.yml
- filename: canonical-landscape-debarchive-api-openapi.yml
  format: yaml
  label: Landscape API
  slug: landscape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-landscape-debarchive-api-openapi.yml
- filename: canonical-assertions-api-openapi.yml
  format: yaml
  label: Canonical Assertions API
  slug: canonical-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-assertions-api-openapi.yml
- filename: canonical-search-api-openapi.yml
  format: yaml
  label: Canonical Search API
  slug: canonical-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-search-api-openapi.yml
- filename: canonical-snaps-api-openapi.yml
  format: yaml
  label: Canonical Snaps API
  slug: canonical-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snaps-api-openapi.yml
- filename: canonical-lxd-rest-api-openapi.yml
  format: yaml
  label: LXD REST API
  slug: lxd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-lxd-rest-api-openapi.yml
- filename: canonical-ubuntu-security-api-openapi.json
  format: json
  label: Ubuntu Security API
  slug: ubuntu-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-ubuntu-security-api-openapi.json
- filename: canonical-pebble-api-openapi.yml
  format: yaml
  label: Pebble API
  slug: pebble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-pebble-api-openapi.yml
- filename: canonical-testflinger-api-openapi.json
  format: json
  label: Testflinger API
  slug: testflinger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-testflinger-api-openapi.json
- filename: canonical-hardware-api-openapi.json
  format: json
  label: Ubuntu Hardware API (hwapi)
  slug: hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-hardware-api-openapi.json
- filename: canonical-identity-platform-api-openapi.yml
  format: yaml
  label: Canonical Identity Platform API
  slug: identity-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-identity-platform-api-openapi.yml
- filename: canonical-test-observer-api-openapi.json
  format: json
  label: Test Observer API
  slug: test-observer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-test-observer-api-openapi.json
- filename: canonical-anbox-cloud-ams-api-openapi.json
  format: json
  label: Anbox Cloud AMS API
  slug: anbox-cloud-ams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-cloud-ams-api-openapi.json
- filename: canonical-anbox-stream-gateway-api-openapi.json
  format: json
  label: Anbox Stream Gateway API
  slug: anbox-stream-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-stream-gateway-api-openapi.json
- filename: canonical-cos-registration-server-api-openapi.yml
  format: yaml
  label: COS Registration Server API
  slug: cos-registration-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-cos-registration-server-api-openapi.yml
- filename: canonical-microceph-api-openapi.yml
  format: yaml
  label: MicroCeph REST API
  slug: microceph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-microceph-api-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Canonical Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Canonical exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Canonical
provider_slug: canonical
slug: canonical-agentic-access
source_filename: canonical-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/canonical-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 7\n    acting: 5\n  by_consequence:\n    read: 7\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/snaps/info/{name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snaps/find\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snaps/refresh\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assertions/{type}/{primaryKey}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/snaps/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/snaps/names\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/snaps/sections\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/snaps/auth/nonces\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/snaps/auth/sessions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/snaps/auth/devices\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/snaps/auth/request-id\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/agentic-access/canonical-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Cloud
- Linux
- Open-Source
- Ubuntu
- Containers
- Bare Metal
- Charms
- Identity
---
