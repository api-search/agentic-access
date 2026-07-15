---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: zdnet-rss.yml
  format: yaml
  label: ZDNet RSS Feed
  slug: rss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zdnet/refs/heads/main/openapi/zdnet-rss.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zdnet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'ZDNet exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ZDNet
provider_slug: zdnet
slug: zdnet-agentic-access
source_filename: zdnet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zdnet-rss.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /news/rss.xml\n  method: get\n  operationId: getNewsRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topic/security/rss.xml\n  method: get\n  operationId: getSecurityRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topic/cloud/rss.xml\n  method: get\n  operationId: getCloudRssFeed\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topic/artificial-intelligence/rss.xml\n  method: get\n  operationId: getAiRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topic/developer/rss.xml\n  method: get\n  operationId: getDeveloperRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topic/innovation/rss.xml\n  method: get\n  operationId: getInnovationRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zdnet/refs/heads/main/agentic-access/zdnet-agentic-access.yml
summary_line: 6 operations
tags:
- Enterprise IT
- Media
- Technology News
---
