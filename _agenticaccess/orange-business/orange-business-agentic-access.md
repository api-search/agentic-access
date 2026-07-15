---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 4
api_specs:
- filename: orange-business-number-verification-openapi.yml
  format: yaml
  label: Orange Business Number Verification API
  slug: orange-business-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-number-verification-openapi.yml
- filename: orange-business-sim-swap-openapi.yml
  format: yaml
  label: Orange Business SIM Swap API
  slug: orange-business-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-sim-swap-openapi.yml
- filename: orange-business-device-swap-openapi.yml
  format: yaml
  label: Orange Business Device Swap API
  slug: orange-business-device-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-swap-openapi.yml
- filename: orange-business-kyc-match-openapi.yml
  format: yaml
  label: Orange Business KYC Match API
  slug: orange-business-kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-kyc-match-openapi.yml
- filename: orange-business-device-location-retrieval-openapi.yml
  format: yaml
  label: Orange Business Device Location Retrieval API
  slug: orange-business-device-location-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-location-retrieval-openapi.yml
- filename: orange-business-device-location-verification-openapi.yml
  format: yaml
  label: Orange Business Device Location Verification API
  slug: orange-business-device-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-location-verification-openapi.yml
- filename: orange-business-geofencing-openapi.yml
  format: yaml
  label: Orange Business Geofencing API
  slug: orange-business-geofencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-geofencing-openapi.yml
- filename: orange-business-device-reachability-status-openapi.yml
  format: yaml
  label: Orange Business Device Reachability Status API
  slug: orange-business-device-reachability-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-reachability-status-openapi.yml
- filename: orange-business-device-roaming-status-openapi.yml
  format: yaml
  label: Orange Business Device Roaming Status API
  slug: orange-business-device-roaming-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-roaming-status-openapi.yml
- filename: orange-business-quality-on-demand-openapi.yml
  format: yaml
  label: Orange Business Quality on Demand API
  slug: orange-business-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-quality-on-demand-openapi.yml
- filename: orange-business-population-density-data-openapi.yml
  format: yaml
  label: Orange Business Population Density Data API
  slug: orange-business-population-density-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-population-density-data-openapi.yml
consequence_counts:
  read: 4
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Orange Business Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Orange Business exposes 21 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Orange Business
provider_slug: orange-business
slug: orange-business-agentic-access
source_filename: orange-business-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/orange-business-device-location-retrieval-openapi.yml, openapi/orange-business-device-location-verification-openapi.yml,\n  openapi/orange-business-device-reachability-status-openapi.yml, openapi/orange-business-device-roaming-status-openapi.yml,\n  openapi/orange-business-device-swap-openapi.yml, openapi/orange-business-geofencing-openapi.yml,\n  openapi/orange-business-kyc-match-openapi.yml, openapi/orange-business-number-verification-openapi.yml,\n  openapi/orange-business-population-density-data-openapi.yml, openapi/orange-business-quality-on-demand-openapi.yml,\n  openapi/orange-business-sim-swap-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n\
  \    acting: 17\n    connected: 4\n  by_consequence:\n    write: 17\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /retrieve\n  method: post\n  operationId: retrieveLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - location-retrieval:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify\n  method: post\n  operationId: verifyLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - location-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId: getReachabilityStatus\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-reachability-status:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId: getRoamingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-roaming-status:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-date\n  method: post\n  operationId: retrieveDeviceSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-swap\n    - device-swap:retrieve-date\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: checkDeviceSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-swap\n    - device-swap:check\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: post\n  operationId: createGeofencingSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - geofencing-subscriptions:org.camaraproject.geofencing-subscriptions.v0.area-entered:create\n    - geofencing-subscriptions:org.camaraproject.geofencing-subscriptions.v0.area-left:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: retrieveGeofencingSubscriptionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - geofencing-subscriptions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}\n  method: get\n  operationId: retrieveGeofencingSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - geofencing-subscriptions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteGeofencingSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - geofencing-subscriptions:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /match\n  method: post\n  operationId: KYC_Match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc-match:match\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify\n  method: post\n  operationId: phoneNumberVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - number-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device-phone-number\n  method: get\n  operationId: phoneNumberShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - number-verification:device-phone-number:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retrieve\n  method: post\n  operationId: retrievePopulationDensity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - population-density-data:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}\n  method: get\n  operationId: getSession\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - quality-on-demand:sessions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/extend\n  method: post\n  operationId: extendQosSessionDuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /retrieve-sessions\n  method: post\n  operationId: retrieveSessionsByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:retrieve-by-device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-date\n  method: post\n  operationId: retrieveSimSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap\n    - sim-swap:retrieve-date\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: checkSimSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - sim-swap\n    - sim-swap:check\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/agentic-access/orange-business-agentic-access.yml
summary_line: 21 operations · 17 acting
tags:
- 5G
- AI
- B2B
- CAMARA
- Cloud
- Communications
- Cybersecurity
- Developer Platform
- Digital Workplace
- Enterprise
- France
- IoT
- Identity
- Mobile Money
- Network APIs
- Open Gateway
- Orange
- Payments
- SD-WAN
- SMS
- SASE
- Telco
- Voice
---
