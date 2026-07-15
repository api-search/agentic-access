---
acting_count: 8
action_class_counts:
  acting: 8
api_specs:
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge PR Review
  slug: qodo-gen-merge-pr-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge Code Suggestions
  slug: qodo-gen-merge-code-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge PR Description
  slug: qodo-gen-merge-describe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge Ask and Chat
  slug: qodo-gen-merge-ask-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Gen Test Generation
  slug: qodo-gen-test-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Command Agent API
  slug: qodo-gen-command-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
consequence_counts:
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qodo Gen Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Qodo exposes 8 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qodo
provider_slug: qodo-gen
slug: qodo-gen-agentic-access
source_filename: qodo-gen-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/qodo-gen-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 8\n  by_consequence:\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /webhook\n  method: post\n  operationId: receiveGitWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pull-requests/review\n  method: post\n  operationId: reviewPullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pull-requests/describe\n  method: post\n  operationId: describePullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pull-requests/improve\n  method: post\n  operationId: improvePullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pull-requests/ask\n  method: post\n  operationId: askPullRequest\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pull-requests/add-docs\n  method: post\n  operationId: addDocs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate/tests\n  method: post\n  operationId: generateTests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent}/run\n  method: post\n\
  \  operationId: runAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/agentic-access/qodo-gen-agentic-access.yml
summary_line: 8 operations · 8 acting
tags:
- AI Coding Assistant
- Code Review
- Test Generation
- Developer Tools
- LLM
- AI
- Pull Request Review
- Code Quality
- Agents
- Open Source
---
