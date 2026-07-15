---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Armor API
  slug: google-cloud-armor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-armor/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Armor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Google Cloud Armor exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Armor
provider_slug: google-cloud-armor
slug: google-cloud-armor-agentic-access
source_filename: google-cloud-armor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 2\n    acting: 5\n  by_consequence:\n    read: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/global/securityPolicies\n  method: get\n  operationId: listSecurityPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/securityPolicies\n  method: post\n  operationId: createSecurityPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/securityPolicies/{securityPolicy}\n  method: get\n  operationId: getSecurityPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/securityPolicies/{securityPolicy}\n  method: patch\n  operationId: patchSecurityPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/securityPolicies/{securityPolicy}\n  method: delete\n  operationId: deleteSecurityPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/securityPolicies/{securityPolicy}/addRule\n  method: post\n  operationId: addSecurityPolicyRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/securityPolicies/{securityPolicy}/removeRule\n\
  \  method: post\n  operationId: removeSecurityPolicyRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/compute\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-armor/refs/heads/main/agentic-access/google-cloud-armor-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- DDoS Protection
- Firewall
- Google Cloud
- Security
- WAF
---
