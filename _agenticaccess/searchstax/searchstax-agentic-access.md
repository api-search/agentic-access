---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: searchstax-provisioning-openapi.yml
  format: yaml
  label: SearchStax Provisioning API
  slug: searchstax-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-provisioning-openapi.yml
consequence_counts:
  physical: 5
  read: 9
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Searchstax Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /account/{account_name}/deployment/{uid}/server/{node}/stop-solr/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/{account_name}/deployment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /account/{account_name}/deployment/{uid}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/{account_name}/deployment/{uid}/backup/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /account/{account_name}/deployment/{uid}/rolling-restart/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/{account_name}/deployment/{uid}/server/{node}/start-solr/
operation_count: 17
overview: 'SearchStax exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 2 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SearchStax
provider_slug: searchstax
slug: searchstax-agentic-access
source_filename: searchstax-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/searchstax-provisioning-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 8\n    connected: 9\n  by_consequence:\n    write: 2\n    read: 9\n    physical: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /obtain-auth-token/\n  method: post\n  operationId: obtainAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_name}/deployment/\n  method: get\n  operationId:\
  \ listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/deployment/\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_name}/deployment/{uid}/\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/deployment/{uid}/\n  method: delete\n  operationId: deleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_name}/deployment/{uid}/deployment-health/\n  method: get\n  operationId: getDeploymentHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/deployment/{uid}/collection-health/\n  method: get\n  operationId: getCollectionHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/deployment/{uid}/rolling-restart/\n  method: put\n  operationId: rollingRestart\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_name}/deployment/{uid}/backup/\n  method: get\n  operationId: listBackups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/deployment/{uid}/backup/\n  method: post\n  operationId: createBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_name}/deployment/{uid}/server/\n  method: get\n  operationId:\
  \ listNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/deployment/{uid}/server/{node}/start-solr/\n  method: post\n  operationId: startSolrNode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_name}/deployment/{uid}/server/{node}/stop-solr/\n  method: post\n  operationId: stopSolrNode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /account/{account_name}/deployment/{uid}/server/{node}/host-status/\n  method: get\n  operationId: getNodeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/plan/\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/usage/{year}/{month}/\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_name}/apikey/\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/agentic-access/searchstax-agentic-access.yml
summary_line: 17 operations · 8 acting · 1 human-in-the-loop
tags:
- Search
- Solr
- Managed Search
- Search Infrastructure
- Full-Text Search
- Site Search
---
