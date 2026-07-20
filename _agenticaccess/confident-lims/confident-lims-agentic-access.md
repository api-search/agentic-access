---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 28
api_specs:
- filename: confident-lims-labs-openapi.json
  format: json
  label: Confident Cannabis API - Lab Endpoints
  slug: confident-cannabis-api-lab-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-labs-openapi.json
- filename: confident-lims-clients-openapi.json
  format: json
  label: Confident Cannabis API - Client Endpoints
  slug: confident-cannabis-api-client-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-clients-openapi.json
- filename: confident-lims-common-openapi.json
  format: json
  label: Confident Cannabis API - Common Reference Data
  slug: confident-cannabis-api-common-reference-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-common-openapi.json
consequence_counts:
  physical: 9
  read: 28
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Confident Lims Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v0/labs/order/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/document
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/status/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/status/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/status/revise
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/status/uncancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/status/unverify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/labs/order/{order_id}/status/verify
operation_count: 45
overview: 'Confident LIMS exposes 45 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 8 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Confident LIMS
provider_slug: confident-lims
slug: confident-lims-agentic-access
source_filename: confident-lims-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/confident-lims-clients-openapi.json, openapi/confident-lims-common-openapi.json,\n  openapi/confident-lims-labs-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 45\n  by_action_class:\n    connected: 28\n    acting: 17\n  by_consequence:\n    read: 28\n    write: 8\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v0/clients/client\n  method: get\n  operationId: getClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/order/{order_id}\n  method: get\n  operationId: getOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/labs\n  method: get\n  operationId: getLabs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/lab/{lab_id}\n  method: get\n  operationId: getLabDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/samples\n  method: get\n  operationId: getSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/sample/{sample_id}\n\
  \  method: get\n  operationId: getSampleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/sampletypes\n  method: get\n  operationId: getClientSampleTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/samplecategories\n  method: get\n  operationId: getClientSampleCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/sampleproductionmethods\n  method: get\n  operationId: getClientSampleProductionMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/clients/sampleclassifications\n  method: get\n  operationId: getClientSampleClassifications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/compounds\n  method: get\n  operationId: getCompounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/testtypes\n  method: get\n  operationId: getTestTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/sampletypes\n  method: get\n  operationId: getSampleTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/samplecategories\n  method: get\n  operationId: getSampleCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v0/sampleproductionmethods\n  method: get\n  operationId: getSampleProductionMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/sampleclassifications\n  method: get\n  operationId: getSampleClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/orderstatuses\n  method: get\n  operationId: getOrderStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/lab\n  method: get\n  operationId: getLab\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/samples\n  method: get\n  operationId: getSamples\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/sample/{sample_id}\n  method: get\n  operationId: getSampleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/sample/{sample_id}\n  method: patch\n  operationId: editSample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/sample/{sample_id}/image\n  method: post\n  operationId: uploadSampleImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/sample/{sample_id}/coa\n  method: post\n  operationId: uploadSampleCOA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/sample/{sample_id}/coa_addition\n  method: post\n  operationId: uploadSampleCOAAddition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/sample/{sample_id}/test_results\n  method: post\n  operationId: submitTestResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/sample/{sample_id}/weight_on_hand\n  method: post\n  operationId: adjustWeightOnHand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/order\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}\n  method: get\n  operationId: getOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/order/{order_id}\n  method: patch\n  operationId: editOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/document\n  method: post\n  operationId: uploadOrderDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/status/verify\n  method: post\n  operationId: verifyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/status/complete\n  method: post\n  operationId: completeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/status/unverify\n  method: post\n  operationId: unverifyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/status/revise\n  method: post\n  operationId: reviseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/status/cancel\n\
  \  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/order/{order_id}/status/uncancel\n  method: post\n  operationId: uncancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labs/testpackages\n  method: get\n  operationId: getTestPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v0/labs/testtypes\n  method: get\n  operationId: getLabTestTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/compounds\n  method: get\n  operationId: getLabCompounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/clients\n  method: get\n  operationId: getClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/clients\n  method: post\n  operationId: createClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v0/labs/client/{client_id}\n  method: get\n  operationId: getClientDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/labs/client/{client_id}/invite\n  method: post\n  operationId: inviteUserToClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/agentic-access/confident-lims-agentic-access.yml
summary_line: 45 operations · 17 acting
tags:
- Company
- LIMS
- Laboratory Information Management
- Analytical Testing
- Cannabis Testing
- Compliance
- Sample Management
- Lab Software
---
