---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 15
api_specs:
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Insureds API
  slug: nowcerts-insureds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Policies API
  slug: nowcerts-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Carriers API
  slug: nowcerts-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Endorsements API
  slug: nowcerts-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Tasks API
  slug: nowcerts-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
consequence_counts:
  read: 15
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nowcerts Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'NowCerts exposes 21 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NowCerts
provider_slug: nowcerts
slug: nowcerts-agentic-access
source_filename: nowcerts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nowcerts-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 6\n    connected: 15\n  by_consequence:\n    write: 6\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Insured/Insert\n  method: post\n  operationId: insertInsured\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /InsuredDetailList\n  method: get\n  operationId: listInsuredDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customers/GetCustomers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Policy/Insert\n  method: post\n  operationId: insertPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /Policy/PartialUpdate\n  method: patch\n  operationId: partialUpdatePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Policy/FindPolicies\n  method: get\n  operationId: findPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PolicyDetailList\n  method: get\n  operationId: listPolicyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Policy/Coverages\n  method: get\n  operationId: getPolicyCoverages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /Policy/StatusTypes\n  method: get\n  operationId: getPolicyStatusTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CarrierDetailList\n  method: get\n  operationId: listCarrierDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /UnderwriterDetailList\n  method: get\n  operationId: listUnderwriterDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LineOfBusinessList\n  method: get\n  operationId: listLineOfBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Policy/InsertWithEndorementId\n  method: post\n  operationId:\
  \ insertPolicyWithEndorsementId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PolicyEndorsementDetailList\n  method: get\n  operationId: listPolicyEndorsementDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PolicyEndorsementAgencyCommissionDetailList\n  method: get\n  operationId: listEndorsementAgencyCommissionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TasksWork/InsertUpdate\n  method: post\n  operationId: insertUpdateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /TasksList\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TasksWorkGroupList\n  method: get\n  operationId: listTaskWorkGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ToDoList\n  method: get\n  operationId: listToDo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /heartbeat\n  method: get\n  operationId: heartbeat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/agentic-access/nowcerts-agentic-access.yml
summary_line: 21 operations · 6 acting
tags:
- Insurance
- Insurtech
- Agency Management System
- AMS
- Policies
- Insureds
- Certificates of Insurance
- REST
---
