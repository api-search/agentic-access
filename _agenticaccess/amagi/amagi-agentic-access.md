---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 12
api_specs:
- filename: amagi-add-user-api-openapi.yml
  format: yaml
  label: Amagi Add User API
  slug: amagi-add-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-add-user-api-openapi.yml
- filename: amagi-cancel-api-openapi.yml
  format: yaml
  label: Amagi Cancel API
  slug: amagi-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-cancel-api-openapi.yml
- filename: amagi-create-customer-api-openapi.yml
  format: yaml
  label: Amagi Create Customer API
  slug: amagi-create-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-create-customer-api-openapi.yml
- filename: amagi-delete-customer-api-openapi.yml
  format: yaml
  label: Amagi Delete Customer API
  slug: amagi-delete-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-delete-customer-api-openapi.yml
- filename: amagi-destroy-api-openapi.yml
  format: yaml
  label: Amagi Destroy API
  slug: amagi-destroy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-destroy-api-openapi.yml
- filename: amagi-disable-user-api-openapi.yml
  format: yaml
  label: Amagi Disable User API
  slug: amagi-disable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-disable-user-api-openapi.yml
- filename: amagi-enable-user-api-openapi.yml
  format: yaml
  label: Amagi Enable User API
  slug: amagi-enable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-enable-user-api-openapi.yml
- filename: amagi-get-info-api-openapi.yml
  format: yaml
  label: Amagi Get Info API
  slug: amagi-get-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-get-info-api-openapi.yml
- filename: amagi-get-key-api-openapi.yml
  format: yaml
  label: Amagi Get Key API
  slug: amagi-get-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-get-key-api-openapi.yml
- filename: amagi-get-metrics-api-openapi.yml
  format: yaml
  label: Amagi Get Metrics API
  slug: amagi-get-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-get-metrics-api-openapi.yml
- filename: amagi-head-key-api-openapi.yml
  format: yaml
  label: Amagi Head Key API
  slug: amagi-head-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-head-key-api-openapi.yml
- filename: amagi-list-api-openapi.yml
  format: yaml
  label: Amagi List API
  slug: amagi-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-list-api-openapi.yml
- filename: amagi-list-keys-api-openapi.yml
  format: yaml
  label: Amagi List Keys API
  slug: amagi-list-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-list-keys-api-openapi.yml
- filename: amagi-list-versions-api-openapi.yml
  format: yaml
  label: Amagi List Versions API
  slug: amagi-list-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-list-versions-api-openapi.yml
- filename: amagi-logs-api-openapi.yml
  format: yaml
  label: Amagi Logs API
  slug: amagi-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-logs-api-openapi.yml
- filename: amagi-regenerate-token-api-openapi.yml
  format: yaml
  label: Amagi Regenerate Token API
  slug: amagi-regenerate-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-regenerate-token-api-openapi.yml
- filename: amagi-retry-api-openapi.yml
  format: yaml
  label: Amagi Retry API
  slug: amagi-retry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-retry-api-openapi.yml
- filename: amagi-set-key-api-openapi.yml
  format: yaml
  label: Amagi Set Key API
  slug: amagi-set-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-set-key-api-openapi.yml
- filename: amagi-status-api-openapi.yml
  format: yaml
  label: Amagi Status API
  slug: amagi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-status-api-openapi.yml
- filename: amagi-submit-api-openapi.yml
  format: yaml
  label: Amagi Submit API
  slug: amagi-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-submit-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Amagi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /disable-user
operation_count: 20
overview: 'Amagi exposes 20 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amagi
provider_slug: amagi
slug: amagi-agentic-access
source_filename: amagi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/amagi-callisto-openapi.yml, openapi/amagi-mapsor-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 8\n    connected: 12\n  by_consequence:\n    write: 7\n    read: 12\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /create-customer\n  method: post\n  operationId: createNewCustomerEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-customer\n  method: post\n  operationId:\
  \ deleteExistingCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /set-key\n  method: post\n  operationId: setKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list-keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-key\n  method: get\n  operationId: getKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /head-key\n  method: get\n  operationId: headKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-versions\n  method: get\n  operationId: listVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add-user\n  method: post\n  operationId: createNewUserEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regenerate-token\n  method: post\n  operationId: regenerateTokenForExistingUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enable-user\n  method: post\n  operationId: enableUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disable-user\n  method: post\n  operationId: disableUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /submit\n  method: post\n  operationId: createContainerJob\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cancel/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retry/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-info/{region}/{instance_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destroy/{region}/{instance_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-metrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/agentic-access/amagi-agentic-access.yml
summary_line: 20 operations · 8 acting · 1 human-in-the-loop
tags:
- Company
- Media
- Broadcast
- Streaming
- Video
- CTV
- FAST
- Advertising
- Cloud
- Playout
---
