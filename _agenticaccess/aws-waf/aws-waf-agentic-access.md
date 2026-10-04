---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: aws-waf-aws-wafv2-api-api-openapi.yml
  format: yaml
  label: AWS WAF AWS WAFV2 API
  slug: aws-waf-aws-wafv2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/openapi/aws-waf-aws-wafv2-api-api-openapi.yml
- filename: aws-waf-ip-sets-api-openapi.yml
  format: yaml
  label: AWS WAF IP Sets API
  slug: aws-waf-ip-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/openapi/aws-waf-ip-sets-api-openapi.yml
- filename: aws-waf-rule-groups-api-openapi.yml
  format: yaml
  label: AWS WAF Rule Groups API
  slug: aws-waf-rule-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/openapi/aws-waf-rule-groups-api-openapi.yml
- filename: aws-waf-web-acls-api-openapi.yml
  format: yaml
  label: AWS WAF Web ACLs API
  slug: aws-waf-web-acls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/openapi/aws-waf-web-acls-api-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aws Waf Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'AWS WAF exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWS WAF
provider_slug: aws-waf
slug: aws-waf-agentic-access
source_filename: aws-waf-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/amazon-waf-ip-sets-api-openapi.yml, openapi/amazon-waf-rule-groups-api-openapi.yml,\n  openapi/amazon-waf-web-acls-api-openapi.yml, openapi/aws-waf-aws-wafv2-api-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /#CreateIPSet\n  method: post\n  operationId: CreateIPSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /#CreateRuleGroup\n  method: post\n  operationId: CreateRuleGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateWebACL\n  method: post\n  operationId: CreateWebACL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetWebACL\n  method: post\n  operationId: GetWebACL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#ListWebACLs\n  method: post\n  operationId: ListWebACLs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: invokeWafv2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-waf/refs/heads/main/agentic-access/aws-waf-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Security
- Web Application Firewall
- DDoS Protection
- Bot Management
- Edge Security
- Cloud
---
