---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 6
consequence_counts:
  read: 6
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Secure Client Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Cisco Secure Client exposes 15 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco Secure Client
provider_slug: cisco-secure-client
slug: cisco-secure-client-agentic-access
source_filename: cisco-secure-client-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cisco-secure-client-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 9\n    connected: 6\n  by_consequence:\n    write: 9\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/fmc_platform/v1/auth/generatetoken\n  method: post\n  operationId: generateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_platform/v1/auth/refreshtoken\n  method: post\n  operationId: refreshToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_config/v1/domain/{domainUUID}/devices/devicerecords\n  method: get\n  operationId: listDeviceRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fmc_config/v1/domain/{domainUUID}/devices/devicerecords\n  method: post\n  operationId: createDeviceRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_config/v1/domain/{domainUUID}/devices/devicerecords/{objectId}\n\
  \  method: get\n  operationId: getDeviceRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fmc_config/v1/domain/{domainUUID}/devices/devicerecords/{objectId}\n  method: put\n  operationId: updateDeviceRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_config/v1/domain/{domainUUID}/devices/devicerecords/{objectId}\n  method: delete\n  operationId: deleteDeviceRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/fmc_config/v1/domain/{domainUUID}/policy/accesspolicies\n  method: get\n  operationId: listAccessPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fmc_config/v1/domain/{domainUUID}/policy/accesspolicies\n  method: post\n  operationId: createAccessPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_config/v1/domain/{domainUUID}/policy/accesspolicies/{containerUUID}/accessrules\n  method: get\n  operationId: listAccessRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fmc_config/v1/domain/{domainUUID}/policy/accesspolicies/{containerUUID}/accessrules\n\
  \  method: post\n  operationId: createAccessRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_config/v1/domain/{domainUUID}/object/networks\n  method: get\n  operationId: listNetworkObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fmc_config/v1/domain/{domainUUID}/object/networks\n  method: post\n  operationId: createNetworkObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fmc_config/v1/domain/{domainUUID}/object/hosts\n\
  \  method: get\n  operationId: listHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fmc_config/v1/domain/{domainUUID}/object/hosts\n  method: post\n  operationId: createHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-secure-client/refs/heads/main/agentic-access/cisco-secure-client-agentic-access.yml
summary_line: 15 operations · 9 acting
tags:
- Endpoint Security
- Remote Access
- Security
- VPN
- Zero Trust
---
