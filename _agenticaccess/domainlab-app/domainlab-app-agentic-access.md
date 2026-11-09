---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: domainlab-app-account-api-openapi.yml
  format: yaml
  label: Domain Lab Account API
  slug: domainlab-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-account-api-openapi.yml
- filename: domainlab-app-alerts-api-openapi.yml
  format: yaml
  label: Domain Lab Alerts API
  slug: domainlab-app-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-alerts-api-openapi.yml
- filename: domainlab-app-domain-status-api-openapi.yml
  format: yaml
  label: Domain Lab Domain Status API
  slug: domainlab-app-domain-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-domain-status-api-openapi.yml
- filename: domainlab-app-domains-api-openapi.yml
  format: yaml
  label: Domain Lab Domains API
  slug: domainlab-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-domains-api-openapi.yml
- filename: domainlab-app-email-api-openapi.yml
  format: yaml
  label: Domain Lab Email API
  slug: domainlab-app-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-email-api-openapi.yml
- filename: domainlab-app-event-types-api-openapi.yml
  format: yaml
  label: Domain Lab Event Types API
  slug: domainlab-app-event-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-event-types-api-openapi.yml
- filename: domainlab-app-events-api-openapi.yml
  format: yaml
  label: Domain Lab Events API
  slug: domainlab-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-events-api-openapi.yml
- filename: domainlab-app-inbox-api-openapi.yml
  format: yaml
  label: Domain Lab Inbox API
  slug: domainlab-app-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-inbox-api-openapi.yml
- filename: domainlab-app-notification-rules-api-openapi.yml
  format: yaml
  label: Domain Lab Notification Rules API
  slug: domainlab-app-notification-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-notification-rules-api-openapi.yml
- filename: domainlab-app-registrar-connections-api-openapi.yml
  format: yaml
  label: Domain Lab Registrar Connections API
  slug: domainlab-app-registrar-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainlab-app/openapi/domainlab-app-registrar-connections-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Domainlab App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /domains/{id}
operation_count: 25
overview: 'Domain Lab exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Domain Lab
provider_slug: domainlab-app
slug: domainlab-app-agentic-access
source_filename: domainlab-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/domainlab-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: post\n  operationId: addDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{id}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}\n  method: patch\n  operationId: updateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{id}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /domains/{id}/scan\n  method: get\n  operationId: getScanHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain-status\n  method: get\n  operationId: checkDomainStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}/events\n  method: get\n  operationId: getDomainEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox\n  method: get\n  operationId: listInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox/read\n  method: post\n  operationId: markInboxRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email\n  method: get\n  operationId: listEmailSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}/email\n  method: get\n  operationId: getDomainEmailSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}/email/history\n  method: get\n  operationId: getDomainEmailSecurityHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}/rescan\n  method: post\n  operationId: rescanDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{id}/ai-review\n  method: post\n  operationId: runAiReview\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{id}/ai-reviews\n  method: get\n  operationId: listAiReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event-types\n  method: get\n  operationId: listEventTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification-rules\n  method: get\n  operationId: listNotificationRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}/alerts\n  method: get\n  operationId: getDomainAlerts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{id}/alerts\n  method: put\n  operationId: updateDomainAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registrar-connections\n  method: get\n  operationId: listRegistrarConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registrar-connections/{id}/sync\n  method: post\n  operationId: syncRegistrarConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/domainlab-app/agentic-access/domainlab-app-agentic-access.yml
summary_line: 25 operations · 8 acting · 1 human-in-the-loop
tags:
- Domain Monitoring
- DNS Monitoring
- SSL Monitoring
- AI Alerts
- Automation Integration
- Webhook Notifications
---
