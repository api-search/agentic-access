---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: sauce.json
  format: json
  label: Sauce Labs Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/sauce.json
- filename: rdc.json
  format: json
  label: Sauce Labs Real Device API
  slug: real-devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/rdc.json
- filename: real-device-access-api-spec.yaml
  format: yaml
  label: Sauce Labs Real Device Access API
  slug: real-device-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/real-device-access-api-spec.yaml
- filename: accounts.yml
  format: yaml
  label: Sauce Labs Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/accounts.yml
- filename: buildsv2.json
  format: json
  label: Sauce Labs Builds API
  slug: builds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/buildsv2.json
- filename: test-authoring-api.json
  format: json
  label: Sauce Labs Test Authoring API
  slug: test-authoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/test-authoring-api.json
- filename: performance.json
  format: json
  label: Sauce Labs Performance API
  slug: performance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/performance.json
consequence_counts:
  read: 10
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Sauce Labs Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/{username}/jobs/{id}/stop
operation_count: 18
overview: 'Sauce Labs exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sauce Labs
provider_slug: sauce-labs
slug: sauce-labs-agentic-access
source_filename: sauce-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sauce-labs-jobs-openapi.yml, openapi/sauce-labs-real-device-access-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 10\n    acting: 8\n  by_consequence:\n    read: 10\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/{username}/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{username}/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/{username}/jobs/{id}\n  method: put\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{username}/jobs/{id}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{username}/jobs/{id}/stop\n  method: put\n  operationId: stopJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/jobs/{id}/{assetName}\n  method: get\n  operationId: getJobAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/info/status\n  method: get\n  operationId: getPlatformStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/info/platforms/{platform}\n  method: get\n  operationId: getPlatformInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.2/users/{username}/concurrency\n  method: get\n  operationId: getUserConcurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/status\n  method: get\n  operationId: getDevicesStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}\n  method: delete\n  operationId: closeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/device/executeShellCommand\n  method: post\n  operationId: executeShellCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/device/installApp\n\
  \  method: post\n  operationId: installApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/device/uninstallApp\n  method: delete\n  operationId: uninstallApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/agentic-access/sauce-labs-agentic-access.yml
summary_line: 18 operations · 8 acting · 1 human-in-the-loop
tags:
- Testing
- Cross-Browser Testing
- Mobile Testing
- Real Devices
- Automation
- CI/CD
- Quality Assurance
---
