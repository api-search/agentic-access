---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks LLM Interactions / Logging API
  slug: llm-interactions-logging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Applications / Versions API
  slug: applications-versions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Annotations API
  slug: annotations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Properties API
  slug: properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deepchecks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Deepchecks exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deepchecks
provider_slug: deepchecks
slug: deepchecks-agentic-access
source_filename: deepchecks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/deepchecks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 7\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/backend-version\n  method: post\n  operationId: getBackendVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/application-versions\n  method: get\n  operationId: listApplicationVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/application-versions\n  method: post\n  operationId: createApplicationVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/application-versions/{application_version_id}/interactions\n  method: post\n  operationId: createInteractions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/application-versions/{application_version_id}/interactions\n  method: get\n  operationId: getInteractionsByFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/application-versions/{application_version_id}/interactions\n  method: delete\n  operationId: deleteInteractions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/application-versions/{application_version_id}/interactions/complete-status\n  method: post\n  operationId: getInteractionCompletionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/application-versions/{application_version_id}/interactions/download\n  method: get\n  operationId: downloadInteractionsByFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{app_id}/llm-prop-definitions\n  method: put\n  operationId: updateLlmPropsDefinitions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/spans\n  method: get\n  operationId: getRawSpansByFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/agentic-access/deepchecks-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- AI
- LLM
- Evaluation
- Testing
- Monitoring
---
