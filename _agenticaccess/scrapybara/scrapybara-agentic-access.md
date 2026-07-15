---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 10
api_specs:
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Instances API
  slug: scrapybara-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Computer Actions API
  slug: scrapybara-computer-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Browser API
  slug: scrapybara-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Code Execution API
  slug: scrapybara-code-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Filesystem API
  slug: scrapybara-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Notebook API
  slug: scrapybara-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Auth States API
  slug: scrapybara-auth-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Environment API
  slug: scrapybara-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 2
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Scrapybara Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /instances/{instance_id}/browser/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /instances/{instance_id}/stop
operation_count: 32
overview: 'Scrapybara exposes 32 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 20 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scrapybara
provider_slug: scrapybara
slug: scrapybara-agentic-access
source_filename: scrapybara-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scrapybara-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 22\n    connected: 10\n  by_consequence:\n    write: 20\n    read: 10\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /start\n  method: post\n  operationId: startInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances\n  method: get\n  operationId: getInstances\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/stop\n  method: post\n  operationId: stopInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /instances/{instance_id}/pause\n  method: post\n  operationId: pauseInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/resume\n  method: post\n  operationId: resumeInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/screenshot\n  method: get\n  operationId: takeScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/stream-url\n  method: get\n  operationId: getStreamUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/computer\n  method: post\n  operationId: runComputerAction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/bash\n  method: post\n  operationId: runBash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/edit\n  method: post\n  operationId: runEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/file\n\
  \  method: post\n  operationId: runFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/browser/start\n  method: post\n  operationId: startBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /instances/{instance_id}/browser/stop\n  method: post\n  operationId: stopBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /instances/{instance_id}/browser/cdp-url\n  method: get\n  operationId: getCdpUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/browser/current-url\n  method: get\n  operationId: getCurrentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/browser/save-auth\n  method: post\n  operationId:\
  \ saveAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/browser/authenticate\n  method: post\n  operationId: authenticateBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/auth-states/{auth_state_id}\n  method: post\n  operationId: modifyAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /auth-states\n  method: get\n  operationId: getAuthStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/code/execute\n  method: post\n  operationId: executeCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/notebooks/kernels\n  method: get\n  operationId: listKernels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/notebooks\n  method: post\n  operationId: createNotebook\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/notebooks/{notebook_id}\n  method: get\n  operationId: getNotebook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/notebooks/{notebook_id}\n  method: delete\n  operationId: deleteNotebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/notebooks/{notebook_id}/cells\n  method: post\n  operationId: addCell\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/notebooks/{notebook_id}/cells/{cell_id}/execute\n  method: post\n  operationId: executeCell\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/notebooks/{notebook_id}/execute\n  method: post\n  operationId: executeNotebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /instances/{instance_id}/env\n  method: get\n  operationId: getEnv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}/env\n  method: post\n  operationId: setEnv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/env\n  method: delete\n  operationId: deleteEnv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/agentic-access/scrapybara-agentic-access.yml
summary_line: 32 operations · 22 acting · 2 human-in-the-loop
tags:
- AI Agents
- Virtual Desktops
- Computer Use
- Browser Automation
- Code Execution
---
