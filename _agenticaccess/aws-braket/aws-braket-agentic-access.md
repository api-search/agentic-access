---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 4
api_specs:
- filename: aws-braket-quantum-tasks-api-openapi.yml
  format: yaml
  label: AWS Braket Quantum Tasks API
  slug: aws-braket-quantum-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-quantum-tasks-api-openapi.yml
- filename: aws-braket-devices-api-openapi.yml
  format: yaml
  label: AWS Braket Devices API
  slug: aws-braket-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-devices-api-openapi.yml
- filename: aws-braket-hybrid-jobs-api-openapi.yml
  format: yaml
  label: AWS Braket Hybrid Jobs API
  slug: aws-braket-hybrid-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-hybrid-jobs-api-openapi.yml
- filename: aws-braket-spending-limits-api-openapi.yml
  format: yaml
  label: AWS Braket Spending Limits API
  slug: aws-braket-spending-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-spending-limits-api-openapi.yml
- filename: aws-braket-tags-api-openapi.yml
  format: yaml
  label: AWS Braket Tags API
  slug: aws-braket-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-tags-api-openapi.yml
consequence_counts:
  read: 4
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aws Braket Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'AWS Braket exposes 17 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWS Braket
provider_slug: aws-braket
slug: aws-braket-agentic-access
source_filename: aws-braket-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aws-braket-devices-api-openapi.yml, openapi/aws-braket-hybrid-jobs-api-openapi.yml,\n  openapi/aws-braket-quantum-tasks-api-openapi.yml, openapi/aws-braket-spending-limits-api-openapi.yml,\n  openapi/aws-braket-tags-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 4\n    acting: 13\n  by_consequence:\n    read: 4\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /device/{deviceArn}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: post\n  operationId:\
  \ searchDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{jobArn}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/{jobArn}/cancel\n  method: put\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: post\n  operationId: searchJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quantum-task\n  method: post\n  operationId: createQuantumTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quantum-task/{quantumTaskArn}\n  method: get\n  operationId: getQuantumTask\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quantum-task/{quantumTaskArn}/cancel\n  method: put\n  operationId: cancelQuantumTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quantum-tasks\n  method: post\n  operationId: searchQuantumTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spending-limit\n  method: post\n  operationId: createSpendingLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spending-limit/{spendingLimitArn}\n  method: put\n  operationId: updateSpendingLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spending-limit/{spendingLimitArn}\n  method: delete\n  operationId: deleteSpendingLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spending-limits\n  method: post\n  operationId: searchSpendingLimits\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{resourceArn}\n  method: get\n  operationId: listTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{resourceArn}\n  method: post\n  operationId: tagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{resourceArn}\n  method: delete\n  operationId: untagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/agentic-access/aws-braket-agentic-access.yml
summary_line: 17 operations · 13 acting
tags:
- Quantum Computing
- QPU
- Simulator
- Hybrid Jobs
- OpenQASM
- PennyLane
- Qiskit
- Quantum
---
