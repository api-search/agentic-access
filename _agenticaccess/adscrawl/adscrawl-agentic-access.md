---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 5
api_specs:
- filename: adscrawl-browser-tasks-api-openapi.yml
  format: yaml
  label: AdsCrawl Browser tasks API
  slug: adscrawl-browser-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/openapi/adscrawl-browser-tasks-api-openapi.yml
- filename: adscrawl-cloud-browsers-api-openapi.yml
  format: yaml
  label: AdsCrawl Cloud browsers API
  slug: adscrawl-cloud-browsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/openapi/adscrawl-cloud-browsers-api-openapi.yml
- filename: adscrawl-remote-cdp-api-openapi.yml
  format: yaml
  label: AdsCrawl Remote CDP API
  slug: adscrawl-remote-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/openapi/adscrawl-remote-cdp-api-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Adscrawl Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cdp/live-token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cdp/sessions/{sessionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cloud-browsers/{id}/stop
operation_count: 15
overview: 'AdsCrawl exposes 15 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 7 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AdsCrawl
provider_slug: adscrawl
slug: adscrawl-agentic-access
source_filename: adscrawl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/adscrawl-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 10\n    connected: 5\n  by_consequence:\n    write: 7\n    read: 5\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /html\n  method: post\n  operationId: renderHtml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenshot\n  method: post\n  operationId: captureScreenshot\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spa-extract\n  method: post\n  operationId: extractSpa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spa-extract/templates\n  method: get\n  operationId: listExtractionTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud-browsers\n  method: get\n  operationId: listCloudBrowsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /cloud-browsers\n  method: post\n  operationId: createCloudBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloud-browsers/launch\n  method: post\n  operationId: launchCloudBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloud-browsers/{id}\n  method: get\n  operationId: getCloudBrowser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud-browsers/{id}/start\n  method:\
  \ post\n  operationId: startCloudBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloud-browsers/{id}/stop\n  method: post\n  operationId: stopCloudBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cdp/sessions\n  method: post\n  operationId: createCdpSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /cdp/sessions\n  method: get\n  operationId: listCdpSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdp/sessions/{sessionId}\n  method: delete\n  operationId: deleteCdpSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cdp/sessions/{sessionId}/json/version\n  method: get\n  operationId: getCdpDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdp/live-token\n  method: post\n  operationId: createLiveControlToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/agentic-access/adscrawl-agentic-access.yml
summary_line: 15 operations · 10 acting · 3 human-in-the-loop
tags:
- Company
- Browser Automation
- WebDataExtraction
- Playwright
- Puppeteer
- CDP
---
