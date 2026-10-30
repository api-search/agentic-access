---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: airtop-profiles-api-openapi.yml
  format: yaml
  label: Airtop Profiles API
  slug: airtop-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-profiles-api-openapi.yml
- filename: airtop-sessions-api-openapi.yml
  format: yaml
  label: Airtop Sessions API
  slug: airtop-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-sessions-api-openapi.yml
- filename: airtop-windows-api-openapi.yml
  format: yaml
  label: Airtop Windows API
  slug: airtop-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-windows-api-openapi.yml
- filename: airtop-agent-director-api-openapi.yml
  format: yaml
  label: Airtop Agent Director API
  slug: airtop-agent-director-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-agent-director-api-openapi.yml
- filename: airtop-agent-folders-api-openapi.yml
  format: yaml
  label: Airtop Agent Folders API
  slug: airtop-agent-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-agent-folders-api-openapi.yml
- filename: airtop-agents-api-openapi.yml
  format: yaml
  label: Airtop Agents API
  slug: airtop-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-agents-api-openapi.yml
- filename: airtop-automations-api-openapi.yml
  format: yaml
  label: Airtop Automations API
  slug: airtop-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-automations-api-openapi.yml
- filename: airtop-beta-api-openapi.yml
  format: yaml
  label: Airtop Beta API
  slug: airtop-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-beta-api-openapi.yml
- filename: airtop-files-api-openapi.yml
  format: yaml
  label: Airtop Files API
  slug: airtop-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-files-api-openapi.yml
- filename: airtop-gtm-engineer-api-openapi.yml
  format: yaml
  label: Airtop GTM Engineer API
  slug: airtop-gtm-engineer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-gtm-engineer-api-openapi.yml
- filename: airtop-knowledge-base-api-openapi.yml
  format: yaml
  label: Airtop Knowledge Base API
  slug: airtop-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-knowledge-base-api-openapi.yml
- filename: airtop-requests-api-openapi.yml
  format: yaml
  label: Airtop Requests API
  slug: airtop-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-requests-api-openapi.yml
- filename: airtop-sensitive-values-api-openapi.yml
  format: yaml
  label: Airtop Sensitive Values API
  slug: airtop-sensitive-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-sensitive-values-api-openapi.yml
- filename: airtop-services-api-openapi.yml
  format: yaml
  label: Airtop Services API
  slug: airtop-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-services-api-openapi.yml
- filename: airtop-team-vault-api-openapi.yml
  format: yaml
  label: Airtop Team Vault API
  slug: airtop-team-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-team-vault-api-openapi.yml
- filename: airtop-templates-api-openapi.yml
  format: yaml
  label: Airtop Templates API
  slug: airtop-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-templates-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 11
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
overview: 'Airtop exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 11 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airtop
provider_slug: airtop
slug: airtop-agentic-access
source_filename: airtop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/airtop-ai-query-api-openapi.yml, openapi/airtop-page-interaction-api-openapi.yml,\n  openapi/airtop-profiles-api-openapi.yml, openapi/airtop-screenshots-api-openapi.yml, openapi/airtop-sessions-api-openapi.yml,\n  openapi/airtop-windows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 12\n    connected: 8\n  by_consequence:\n    write: 11\n    read: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /sessions/{sessionId}/windows/{windowId}/scrape\n  method: post\n  operationId: scrapeContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/page-query\n  method: post\n  operationId: pageQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows/{windowId}/paginated-extraction\n  method: post\n  operationId: paginatedExtraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows/{windowId}/click\n  method: post\n  operationId: click\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/hover\n  method: post\n  operationId: hover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/type\n  method: post\n  operationId: type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/scroll\n  method: post\n  operationId: scroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/profile\n  method: put\n  operationId: saveProfileOnTermination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profileId}\n  method: delete\n  operationId: deleteProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/screenshot\n  method: get\n  operationId: takeScreenshot\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}\n  method: delete\n  operationId: terminateSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /requests/{requestId}\n  method: get\n  operationId: getRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows\n  method: get\n  operationId: listWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows\n  method: post\n  operationId: createWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}\n  method: get\n  operationId: getWindowInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/windows/{windowId}\n  method: delete\n  operationId: closeWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/windows/{windowId}/load-url\n  method: post\n  operationId: loadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/agentic-access/airtop-agentic-access.yml
summary_line: 20 operations · 12 acting · 1 human-in-the-loop
tags:
- Browser Automation
- AI Agents
- Cloud Browser
- Web Scraping
- Headless Chrome
---
