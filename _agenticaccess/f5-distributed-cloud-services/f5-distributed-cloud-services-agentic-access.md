---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 11
api_specs:
- filename: f5-distributed-cloud-services-openapi.yml
  format: yaml
  label: F5 Distributed Cloud Services API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-distributed-cloud-services/refs/heads/main/openapi/f5-distributed-cloud-services-openapi.yml
consequence_counts:
  read: 11
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: F5 Distributed Cloud Services Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'F5 Distributed Cloud Services exposes 21 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: F5 Distributed Cloud Services
provider_slug: f5-distributed-cloud-services
slug: f5-distributed-cloud-services-agentic-access
source_filename: f5-distributed-cloud-services-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/f5-distributed-cloud-services-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 11\n    acting: 10\n  by_consequence:\n    read: 11\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/config/namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces\n  method: post\n  operationId: createNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}\n  method: get\n  operationId: getNamespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces/{namespace}\n  method: delete\n  operationId: deleteNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/http_loadbalancers\n  method: get\n  operationId: listHttpLoadBalancers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/config/namespaces/{namespace}/http_loadbalancers\n  method: post\n  operationId: createHttpLoadBalancer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/http_loadbalancers/{name}\n  method: get\n  operationId: getHttpLoadBalancer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces/{namespace}/http_loadbalancers/{name}\n  method: put\n  operationId: replaceHttpLoadBalancer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/http_loadbalancers/{name}\n  method: delete\n  operationId: deleteHttpLoadBalancer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/tcp_loadbalancers\n  method: get\n  operationId: listTcpLoadBalancers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces/{namespace}/tcp_loadbalancers\n  method: post\n  operationId: createTcpLoadBalancer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/origin_pools\n  method: get\n  operationId: listOriginPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces/{namespace}/origin_pools\n  method: post\n  operationId: createOriginPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/origin_pools/{name}\n  method: get\n  operationId: getOriginPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/config/namespaces/{namespace}/origin_pools/{name}\n  method: delete\n  operationId: deleteOriginPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/app_firewalls\n  method: get\n  operationId: listAppFirewalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces/{namespace}/app_firewalls\n  method: post\n  operationId: createAppFirewall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/config/namespaces/{namespace}/certificates\n  method: get\n  operationId: listCertificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config/namespaces/{namespace}/certificates\n  method: post\n  operationId: createCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/config/namespaces/{namespace}/dns_domains\n  method: get\n  operationId: listDnsDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/namespaces/{namespace}/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-distributed-cloud-services/refs/heads/main/agentic-access/f5-distributed-cloud-services-agentic-access.yml
summary_line: 21 operations · 10 acting
tags:
- Application Security
- Web Application Firewall
- API Security
- Multi-Cloud Networking
- DDoS Protection
- Bot Defense
- Load Balancing
- Edge Compute
---
