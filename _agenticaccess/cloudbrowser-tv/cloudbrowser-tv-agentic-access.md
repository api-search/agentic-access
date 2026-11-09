---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 9
api_specs:
- filename: cloudbrowser-tv-b-api-openapi.yml
  format: yaml
  label: Cloudbrowser B API
  slug: cloudbrowser-tv-b-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudbrowser-tv/openapi/cloudbrowser-tv-b-api-openapi.yml
- filename: cloudbrowser-tv-billing-api-openapi.yml
  format: yaml
  label: Cloudbrowser Billing API
  slug: cloudbrowser-tv-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudbrowser-tv/openapi/cloudbrowser-tv-billing-api-openapi.yml
- filename: cloudbrowser-tv-browsers-api-openapi.yml
  format: yaml
  label: Cloudbrowser Browsers API
  slug: cloudbrowser-tv-browsers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudbrowser-tv/openapi/cloudbrowser-tv-browsers-api-openapi.yml
- filename: cloudbrowser-tv-library-api-openapi.yml
  format: yaml
  label: Cloudbrowser Library API
  slug: cloudbrowser-tv-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudbrowser-tv/openapi/cloudbrowser-tv-library-api-openapi.yml
- filename: cloudbrowser-tv-operations-api-openapi.yml
  format: yaml
  label: Cloudbrowser Operations API
  slug: cloudbrowser-tv-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudbrowser-tv/openapi/cloudbrowser-tv-operations-api-openapi.yml
- filename: cloudbrowser-tv-usage-api-openapi.yml
  format: yaml
  label: Cloudbrowser Usage API
  slug: cloudbrowser-tv-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudbrowser-tv/openapi/cloudbrowser-tv-usage-api-openapi.yml
consequence_counts:
  physical: 4
  read: 9
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudbrowser Tv Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /browsers/{browserId}/grants/{grantId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/plan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/portal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/refresh
operation_count: 29
overview: 'Cloudbrowser exposes 29 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 15 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudbrowser
provider_slug: cloudbrowser-tv
slug: cloudbrowser-tv-agentic-access
source_filename: cloudbrowser-tv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/cloudbrowser-tv-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 20\n    connected: 9\n  by_consequence:\n    write: 15\n    read: 9\n    safety-critical: 1\n    physical: 4\n  human_in_the_loop_required: 1\noperations:\n- path: /browsers\n  method: post\n  operationId: createBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers\n  method: get\n  operationId: listBrowsers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browsers/{browserId}\n  method: get\n  operationId: getBrowser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browsers/{browserId}\n  method: delete\n  operationId: deleteBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/pause\n  method: post\n  operationId: pauseBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/resume\n  method: post\n  operationId: resumeBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/fork\n  method: post\n  operationId: forkBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/grants\n  method: post\n  operationId: createGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/grants\n  method: get\n  operationId: listGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browsers/{browserId}/grants/{grantId}\n  method: delete\n  operationId: revokeGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /browsers/{browserId}/grants/{grantId}\n  method: patch\n  operationId: updateLiveViewLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operations/{operationId}\n  method: get\n  operationId: getOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{browserId}/session/exchange\n  method: post\n  operationId: exchangeViewerTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{browserId}/session/refresh\n  method: post\n\
  \  operationId: refreshViewerSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{browserId}/session/logout\n  method: post\n  operationId: logoutViewerSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/grants/{grantId}/sessions\n  method: get\n  operationId: listLiveViewSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browsers/{browserId}/grants/{grantId}/sessions\n  method:\
  \ delete\n  operationId: endLiveViewSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /library/browsers\n  method: get\n  operationId: listBrowserLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /library/shares/accept\n  method: post\n  operationId: acceptSharedBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /library/browsers/{browserId}\n  method: delete\n  operationId: removeSharedBrowser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /library/browsers/{browserId}/viewer-ticket\n  method: post\n  operationId: createLibraryViewerTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/status\n  method: get\n  operationId: getBillingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/portal\n  method: post\n  operationId: createBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/refresh\n  method: post\n  operationId: refreshBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/upgrade-preview\n  method: post\n  operationId: previewUpgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/plan\n  method: post\n  operationId: changePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browsers/{browserId}/grants/{grantId}/secret\n  method: get\n  operationId: revealGrantSecret\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cloudbrowser-tv/agentic-access/cloudbrowser-tv-agentic-access.yml
summary_line: 29 operations · 20 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Browser
- Cloud
- Chrome
- Automation
---
