---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 6
api_specs:
- filename: airtop-openapi.yml
  format: yaml
  label: Airtop Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-openapi.yml
- filename: airtop-openapi.yml
  format: yaml
  label: Airtop Windows API
  slug: windows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-openapi.yml
- filename: airtop-openapi.yml
  format: yaml
  label: Airtop Page Interaction API
  slug: page-interaction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-openapi.yml
- filename: airtop-openapi.yml
  format: yaml
  label: Airtop AI Query and Extraction API
  slug: ai-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-openapi.yml
- filename: airtop-openapi.yml
  format: yaml
  label: Airtop Screenshots API
  slug: screenshots
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-openapi.yml
- filename: airtop-openapi.yml
  format: yaml
  label: Airtop Profiles API
  slug: profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Airtop Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /sessions/{sessionId}
operation_count: 20
overview: 'Airtop exposes 20 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 13 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airtop
provider_slug: airtop
slug: airtop-agentic-access
source_filename: airtop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/airtop-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 6\n    acting: 14\n  by_consequence:\n    read: 6\n    write: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}\n  method: delete\n  operationId: terminateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sessions/{sessionId}/profile\n  method: put\n  operationId: saveProfileOnTermination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows\n  method: get\n  operationId: listWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows\n  method: post\n  operationId: createWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}\n  method: get\n  operationId: getWindowInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows/{windowId}\n  method: delete\n  operationId: closeWindow\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/load-url\n  method: post\n  operationId: loadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/click\n  method: post\n  operationId: click\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/hover\n  method: post\n  operationId: hover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/type\n  method: post\n  operationId: type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/scroll\n  method: post\n  operationId: scroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/screenshot\n  method: get\n  operationId: takeScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows/{windowId}/scrape\n  method: post\n  operationId: scrapeContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/page-query\n  method: post\n  operationId: pageQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/paginated-extraction\n  method: post\n  operationId: paginatedExtraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profileId}\n  method: delete\n  operationId: deleteProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /requests/{requestId}\n  method: get\n  operationId: getRequestStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/agentic-access/airtop-agentic-access.yml
summary_line: 20 operations · 14 acting · 1 human-in-the-loop
tags:
- Browser Automation
- AI Agents
- Cloud Browser
- Web Scraping
- Headless Chrome
---
