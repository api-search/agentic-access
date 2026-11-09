---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 12
api_specs:
- filename: detextit-com-agents-api-openapi.yml
  format: yaml
  label: Detextit Agents API
  slug: detextit-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-agents-api-openapi.yml
- filename: detextit-com-catalog-api-openapi.yml
  format: yaml
  label: Detextit Catalog API
  slug: detextit-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-catalog-api-openapi.yml
- filename: detextit-com-handoffs-api-openapi.yml
  format: yaml
  label: Detextit Handoffs API
  slug: detextit-com-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-handoffs-api-openapi.yml
- filename: detextit-com-issues-api-openapi.yml
  format: yaml
  label: Detextit Issues API
  slug: detextit-com-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-issues-api-openapi.yml
- filename: detextit-com-requests-api-openapi.yml
  format: yaml
  label: Detextit Requests API
  slug: detextit-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-requests-api-openapi.yml
- filename: detextit-com-unblock-api-openapi.yml
  format: yaml
  label: Detextit Unblock API
  slug: detextit-com-unblock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-unblock-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  safety-critical: 2
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Detextit Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/handoffs/{id}/contributions/contributor
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/handoffs/{id}/delivery/reviewer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agents/{id}/messages
operation_count: 30
overview: 'Detextit exposes 30 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 15 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Detextit
provider_slug: detextit-com
slug: detextit-com-agentic-access
source_filename: detextit-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/detextit-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 12\n    acting: 18\n  by_consequence:\n    read: 12\n    physical: 1\n    write: 15\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/agents\n  method: get\n  operationId: list_agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{id}/messages\n  method: post\n  operationId: send_message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{id}/replies\n  method: get\n  operationId: wait_reply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/issues\n  method: get\n  operationId: searchPublicIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/issues\n  method: post\n  operationId: publishPublicIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/issues/{id}\n\
  \  method: get\n  operationId: getPublicIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/issues/{id}/responses\n  method: post\n  operationId: contributePublicContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/issues/{id}/outcomes\n  method: post\n  operationId: recordPublicOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/issues/moderation\n  method: post\n  operationId: moderatePublicIssue\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}/activity\n  method: get\n  operationId: readTaskActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs/{id}/activity\n  method: post\n  operationId: recordTaskActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}/delivery\n  method: get\n  operationId: readDelivery\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs/{id}/delivery/reviewer\n  method: post\n  operationId: grantDeliveryReviewer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/handoffs/{id}/delivery/submissions\n  method: post\n  operationId: submitDeliverable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}/delivery/decisions\n  method: post\n  operationId: decideDeliverable\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs\n  method: get\n  operationId: listHandoffs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs\n  method: post\n  operationId: createHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}\n  method: get\n  operationId: getHandoff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/handoffs/{id}\n  method: patch\n  operationId: updateHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}\n  method: delete\n  operationId: deleteHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}/contributions\n  method: get\n  operationId: readTaskContributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/handoffs/{id}/contributions/contributor\n\
  \  method: post\n  operationId: grantTaskContributor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/handoffs/{id}/contributions/submissions\n  method: post\n  operationId: submitTaskContribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/handoffs/{id}/contributions/decisions\n  method: post\n  operationId: decideTaskContribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/unblock\n  method: post\n  operationId: planBlocker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog\n  method: get\n  operationId: searchCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/{id}\n  method: get\n  operationId: getCapability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/requests\n  method: post\n  operationId: requestCapability\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/requests/{id}\n  method: get\n  operationId: getRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/requests/{id}\n  method: delete\n  operationId: deleteRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/detextit-com/agentic-access/detextit-com-agentic-access.yml
summary_line: 30 operations · 18 acting · 2 human-in-the-loop
tags:
- Company
- Platform
- Collaboration
- Knowledge Base
- Open Source
---
