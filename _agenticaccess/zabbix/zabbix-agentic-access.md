---
acting_count: 20
action_class_counts:
  acting: 20
api_specs:
- filename: zabbix-actions-api-openapi.yml
  format: yaml
  label: Zabbix Actions API
  slug: zabbix-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-actions-api-openapi.yml
- filename: zabbix-authentication-api-openapi.yml
  format: yaml
  label: Zabbix Authentication API
  slug: zabbix-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-authentication-api-openapi.yml
- filename: zabbix-events-api-openapi.yml
  format: yaml
  label: Zabbix Events API
  slug: zabbix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-events-api-openapi.yml
- filename: zabbix-history-api-openapi.yml
  format: yaml
  label: Zabbix History API
  slug: zabbix-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-history-api-openapi.yml
- filename: zabbix-host-groups-api-openapi.yml
  format: yaml
  label: Zabbix Host Groups API
  slug: zabbix-host-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-host-groups-api-openapi.yml
- filename: zabbix-hosts-api-openapi.yml
  format: yaml
  label: Zabbix Hosts API
  slug: zabbix-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-hosts-api-openapi.yml
- filename: zabbix-items-api-openapi.yml
  format: yaml
  label: Zabbix Items API
  slug: zabbix-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-items-api-openapi.yml
- filename: zabbix-problems-api-openapi.yml
  format: yaml
  label: Zabbix Problems API
  slug: zabbix-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-problems-api-openapi.yml
- filename: zabbix-triggers-api-openapi.yml
  format: yaml
  label: Zabbix Triggers API
  slug: zabbix-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-triggers-api-openapi.yml
- filename: zabbix-users-api-openapi.yml
  format: yaml
  label: Zabbix Users API
  slug: zabbix-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-users-api-openapi.yml
consequence_counts:
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zabbix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Zabbix exposes 20 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zabbix
provider_slug: zabbix
slug: zabbix-agentic-access
source_filename: zabbix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zabbix-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 20\n  by_consequence:\n    write: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: user-login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user.logout\n  method: post\n  operationId: user-logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /host.get\n  method: post\n  operationId: host-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /host.create\n  method: post\n  operationId: host-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /host.update\n  method: post\n  operationId: host-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /host.delete\n  method: post\n  operationId: host-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hostgroup.get\n  method: post\n  operationId: hostgroup-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hostgroup.create\n  method: post\n  operationId: hostgroup-create\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item.get\n  method: post\n  operationId: item-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item.create\n  method: post\n  operationId: item-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trigger.get\n  method: post\n  operationId: trigger-get\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trigger.create\n  method: post\n  operationId: trigger-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event.get\n  method: post\n  operationId: event-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event.acknowledge\n  method: post\n  operationId:\
  \ event-acknowledge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /problem.get\n  method: post\n  operationId: problem-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /action.get\n  method: post\n  operationId: action-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /action.create\n\
  \  method: post\n  operationId: action-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user.get\n  method: post\n  operationId: user-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user.create\n  method: post\n  operationId: user-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /history.get\n  method: post\n  operationId: history-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/agentic-access/zabbix-agentic-access.yml
summary_line: 20 operations · 20 acting
tags:
- Monitoring
- Infrastructure
- Networks
- Alerting
- Open-Source
- Observability
---
