---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 2
api_specs:
- filename: marriott-actuator-api-openapi.yml
  format: yaml
  label: Marriott International Actuator API
  slug: marriott-actuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-actuator-api-openapi.yml
- filename: marriott-auth-api-openapi.yml
  format: yaml
  label: Marriott International Auth API
  slug: marriott-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-auth-api-openapi.yml
- filename: marriott-data-api-openapi.yml
  format: yaml
  label: Marriott International Data API
  slug: marriott-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-api-openapi.yml
- filename: marriott-data-collection-event-api-openapi.yml
  format: yaml
  label: Marriott International Data Collection Event API
  slug: marriott-data-collection-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-collection-event-api-openapi.yml
- filename: marriott-freedompay-freeway-service-api-openapi.yml
  format: yaml
  label: Marriott International FreedomPay Freeway Service API
  slug: marriott-freedompay-freeway-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-freedompay-freeway-service-api-openapi.yml
- filename: marriott-guest-validation-api-openapi.yml
  format: yaml
  label: Marriott International Guest Validation API
  slug: marriott-guest-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-guest-validation-api-openapi.yml
- filename: marriott-internet-purchase-update-api-openapi.yml
  format: yaml
  label: Marriott International Internet Purchase Update API
  slug: marriott-internet-purchase-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-internet-purchase-update-api-openapi.yml
- filename: marriott-landing-page-api-openapi.yml
  format: yaml
  label: Marriott International Landing Page API
  slug: marriott-landing-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-landing-page-api-openapi.yml
- filename: marriott-loyalty-api-openapi.yml
  format: yaml
  label: Marriott International Loyalty API
  slug: marriott-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-loyalty-api-openapi.yml
- filename: marriott-postpreviewsubmit-api-openapi.yml
  format: yaml
  label: Marriott International Post Preview Submit API
  slug: marriott-postpreviewsubmit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-postpreviewsubmit-api-openapi.yml
- filename: marriott-retrieveconfigsmonitoredbyconfigwatcher-api-openapi.yml
  format: yaml
  label: Marriott International Retrieve Configs Monitored By Config Watcher API
  slug: marriott-retrieveconfigsmonitoredbyconfigwatcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-retrieveconfigsmonitoredbyconfigwatcher-api-openapi.yml
- filename: marriott-status-api-openapi.yml
  format: yaml
  label: Marriott International Status API
  slug: marriott-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-status-api-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Marriott Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /actuator/loggers/ROOT
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /loyalty/v1/account-merge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partners/v1/internet-portal/purchase-update
operation_count: 13
overview: 'Marriott International exposes 13 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 8 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Marriott International
provider_slug: marriott
slug: marriott-agentic-access
source_filename: marriott-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: generated\nsource: openapi/marriott-commerce-payment-processor-api-openapi.json, openapi/marriott-data-collection-api-openapi.json,\n  openapi/marriott-finance-status-notifier-api-openapi.json, openapi/marriott-hotel-operations-ara-api-openapi.json,\n  openapi/marriott-loyalty-account-merge-api-openapi.json, openapi/marriott-tip-internet-portal-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 11\n    connected: 2\n  by_consequence:\n    write: 8\n    read: 2\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /freeway/service\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    scope:\n    - MANAGE_ACCT_AUTH_E\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /osd/v1/stays/{confirmation-number}/data-collection\n  method: post\n  operationId: DataCollectionEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: put\n  operationId: updateProcessingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    -\
  \ write\n- path: /retrieveConfigsMonitoredByConfigWatcher\n  method: get\n  operationId: retrieveConfigsMonitoredByConfigWatcher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - write\n- path: /actuator/loggers/ROOT\n  method: post\n  operationId: changeLogger\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - write\n- path: /data\n  method: post\n  operationId: createAdapterProcessingStatusPefTestData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - write\n- path: /data\n  method: delete\n  operationId: deletePerfTestData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - write\n- path: /v1/hotelops/ara/preview-submit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loyalty/v1/account-merge\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/ent-auth/sso/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/v1/internet-portal/landing-page\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/v1/internet-portal/guest-validation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/v1/internet-portal/purchase-update\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/agentic-access/marriott-agentic-access.yml
summary_line: 13 operations · 11 acting · 1 human-in-the-loop
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Distribution
- Loyalty
- Short Term Rental
- Corporate Travel
---
