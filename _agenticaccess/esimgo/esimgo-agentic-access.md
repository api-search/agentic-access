---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 16
api_specs:
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Catalogue API
  slug: catalogue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go eSIMs API
  slug: esims
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Network API
  slug: network
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
consequence_counts:
  physical: 3
  read: 16
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Esimgo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /esims/{iccid}/bundles/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /esims/{iccid}/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inventory/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 22
overview: 'eSIM Go exposes 22 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 2 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: eSIM Go
provider_slug: esimgo
slug: esimgo-agentic-access
source_filename: esimgo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/esimgo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 16\n    acting: 6\n  by_consequence:\n    read: 16\n    physical: 3\n    write: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /catalogue\n  method: get\n  operationId: getCatalogue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogue/{bundleName}\n  method: get\n  operationId: getCatalogueBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderReference}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims\n  method: get\n  operationId: listEsims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /esims\n  method: put\n  operationId: updateEsim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /esims/{iccid}\n  method: get\n  operationId: getEsim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/apply\n  method: post\n  operationId: applyBundleToEsim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /esims/assignments\n  method: get\n  operationId: getEsimInstallDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{iccid}/history\n  method: get\n  operationId: getEsimHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{iccid}/location\n  method: get\n  operationId: getEsimLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{iccid}/sms\n  method: post\n  operationId: sendEsimSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /esims/{iccid}/bundles\n  method: get\n  operationId: listEsimBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{iccid}/bundles/{name}\n  method: get\n  operationId: getEsimBundleStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{iccid}/bundles/{name}\n  method: delete\n  operationId: revokeEsimBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /esims/{iccid}/compatible-bundle\n  method: get\n  operationId: checkBundleCompatibility\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory\n  method: get\n  operationId: getInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/refund\n  method: post\n  operationId: refundInventoryBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networks\n  method: get\n  operationId: getNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation\n  method: get\n  operationId: getOrganisation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/groups\n  method: get\n  operationId: getBundleGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/agentic-access/esimgo-agentic-access.yml
summary_line: 22 operations · 6 acting · 1 human-in-the-loop
tags:
- eSIM
- Connectivity
- Travel Data
- Telecom
- Mobile
---
