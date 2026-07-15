---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 10
api_specs:
- filename: number-verification-openapi.yml
  format: yaml
  label: CAMARA Number Verification API
  slug: number-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/number-verification-openapi.yml
- filename: sim-swap-openapi.yml
  format: yaml
  label: CAMARA SIM Swap API
  slug: sim-swap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/sim-swap-openapi.yml
- filename: device-location-retrieval-openapi.yml
  format: yaml
  label: CAMARA Device Location API
  slug: device-location
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/device-location-retrieval-openapi.yml
- filename: quality-on-demand-openapi.yml
  format: yaml
  label: CAMARA Quality on Demand API
  slug: quality-on-demand
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/quality-on-demand-openapi.yml
- filename: device-status-connected-network-type-openapi.yml
  format: yaml
  label: CAMARA Device Status API
  slug: device-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/device-status-connected-network-type-openapi.yml
- filename: kyc-match-openapi.yml
  format: yaml
  label: CAMARA Know Your Customer API
  slug: know-your-customer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/kyc-match-openapi.yml
- filename: one-time-password-sms-openapi.yml
  format: yaml
  label: CAMARA One Time Password SMS API
  slug: one-time-password-sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/one-time-password-sms-openapi.yml
- filename: device-swap-openapi.yml
  format: yaml
  label: CAMARA Device Swap API
  slug: device-swap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/device-swap-openapi.yml
- filename: simple-edge-discovery-openapi.yml
  format: yaml
  label: CAMARA Simple Edge Discovery API
  slug: simple-edge-discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/simple-edge-discovery-openapi.yml
- filename: carrier-billing-openapi.yml
  format: yaml
  label: CAMARA Carrier Billing Checkout API
  slug: carrier-billing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/carrier-billing-openapi.yml
- filename: population-density-data-openapi.yml
  format: yaml
  label: CAMARA Population Density Data API
  slug: population-density-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/population-density-data-openapi.yml
- filename: home-devices-qod-openapi.yml
  format: yaml
  label: CAMARA Home Devices Quality on Demand API
  slug: home-devices-qod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/home-devices-qod-openapi.yml
- filename: call-forwarding-signal-openapi.yml
  format: yaml
  label: CAMARA Call Forwarding Signal API
  slug: call-forwarding-signal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/call-forwarding-signal-openapi.yml
- filename: sms-openapi.yml
  format: yaml
  label: CAMARA Short Message Service API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/sms-openapi.yml
- filename: connectivity-insights-openapi.yml
  format: yaml
  label: CAMARA Connectivity Insights API
  slug: connectivity-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/openapi/connectivity-insights-openapi.yml
consequence_counts:
  physical: 8
  read: 10
  safety-critical: 1
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Camara Project Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /qos-assignments/{assignmentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /qos-assignments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send-code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /short-message
operation_count: 49
overview: 'CAMARA Project exposes 49 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 30 write, 8 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CAMARA Project
provider_slug: camara-project
slug: camara-project-agentic-access
source_filename: camara-project-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/call-forwarding-signal-openapi.yml, openapi/carrier-billing-openapi.yml, openapi/connectivity-insights-openapi.yml,\n  openapi/device-location-geofencing-openapi.yml, openapi/device-location-retrieval-openapi.yml,\n  openapi/device-location-verification-openapi.yml, openapi/device-status-connected-network-type-openapi.yml,\n  openapi/device-status-reachability-openapi.yml, openapi/device-status-roaming-openapi.yml,\n  openapi/device-swap-openapi.yml, openapi/home-devices-qod-openapi.yml, openapi/kyc-age-verification-openapi.yml,\n  openapi/kyc-fill-in-openapi.yml, openapi/kyc-match-openapi.yml, openapi/number-verification-openapi.yml,\n  openapi/one-time-password-sms-openapi.yml, openapi/population-density-data-openapi.yml, openapi/qos-profiles-openapi.yml,\n  openapi/qos-provisioning-openapi.yml, openapi/quality-on-demand-openapi.yml, openapi/sim-swap-openapi.yml,\n  openapi/sim-swap-subscriptions-openapi.yml, openapi/simple-edge-discovery-openapi.yml,\
  \ openapi/sms-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 39\n    connected: 10\n  by_consequence:\n    write: 30\n    physical: 8\n    read: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /unconditional-call-forwardings\n  method: post\n  operationId: retrieveUnconditionalCallForwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - call-forwarding-signal:unconditional-call-forwardings:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /call-forwardings\n  method:\
  \ post\n  operationId: retrieveCallForwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - call-forwarding-signal:call-forwardings:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carrier-billing:payments:create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: get\n  operationId: retrievePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - carrier-billing:payments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}\n  method: get\n  operationId: retrievePayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carrier-billing:payments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/prepare\n  method: post\n  operationId: preparePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carrier-billing:payments:create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/validate\n  method: post\n  operationId: validatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    scope:\n    - carrier-billing:payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/confirm\n  method: post\n  operationId: confirmPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carrier-billing:payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carrier-billing:payments:write\n   \
  \ audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-network-quality\n  method: post\n  operationId: checkNetworkQuality\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connectivity-insights:check\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: post\n  operationId: createGeofencingSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - geofencing-subscriptions:org.camaraproject.geofencing-subscriptions.v0.area-entered:create\n    - geofencing-subscriptions:org.camaraproject.geofencing-subscriptions.v0.area-left:create\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: retrieveGeofencingSubscriptionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - geofencing-subscriptions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}\n  method: get\n  operationId: retrieveGeofencingSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - geofencing-subscriptions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteGeofencingSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - geofencing-subscriptions:delete\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId: retrieveLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - location-retrieval:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify\n  method: post\n  operationId: verifyLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - location-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId:\
  \ getConnectedNetworkType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connected-network-type:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId: getReachabilityStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-reachability-status:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId: getRoamingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-roaming-status:read\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-date\n  method: post\n  operationId: retrieveDeviceSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-swap\n    - device-swap:retrieve-date\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: checkDeviceSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-swap\n    - device-swap:check\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qos\n  method: put\n  operationId: setQos\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - home-devices-qod:qos:write\n- path: /verify\n  method: post\n  operationId: verifyAge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc-age-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fill-in\n  method: post\n  operationId: KYC_Fill-in\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc-fill-in:address\n    - kyc-fill-in:birthdate\n    - kyc-fill-in:country\n    - kyc-fill-in:email\n    - kyc-fill-in:familyName\n\
  \    - kyc-fill-in:familyNameAtBirth\n    - kyc-fill-in:gender\n    - kyc-fill-in:givenName\n    - kyc-fill-in:houseNumberExtension\n    - kyc-fill-in:idDocument\n    - kyc-fill-in:locality\n    - kyc-fill-in:middleNames\n    - kyc-fill-in:name\n    - kyc-fill-in:nameKanaHankaku\n    - kyc-fill-in:nameKanaZenkaku\n    - kyc-fill-in:phoneNumber\n    - kyc-fill-in:postalCode\n    - kyc-fill-in:region\n    - kyc-fill-in:set-all\n    - kyc-fill-in:streetName\n    - kyc-fill-in:streetNumber\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /match\n  method: post\n  operationId: KYC_Match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc-match:match\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /verify\n  method: post\n  operationId: phoneNumberVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - number-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device-phone-number\n  method: get\n  operationId: phoneNumberShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - number-verification:device-phone-number:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /send-code\n  method: post\n  operationId: sendCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - one-time-password-sms:send-validate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate-code\n  method: post\n  operationId: validateCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - one-time-password-sms:send-validate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve\n  method: post\n  operationId: retrievePopulationDensity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - population-density-data:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-qos-profiles\n\
  \  method: post\n  operationId: retrieveQoSProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - qos-profiles:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qos-profiles/{name}\n  method: get\n  operationId: getQosProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - qos-profiles:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qos-assignments\n  method: post\n  operationId: createQosAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - qos-provisioning:qos-assignments:create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qos-assignments/{assignmentId}\n  method: get\n  operationId: getQosAssignmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - qos-provisioning:qos-assignments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qos-assignments/{assignmentId}\n  method: delete\n  operationId: revokeQosAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - qos-provisioning:qos-assignments:delete\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /retrieve-qos-assignment\n  method: post\n  operationId: getQosAssignmentByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - qos-provisioning:qos-assignments:read-by-device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - quality-on-demand:sessions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}\n  method: delete\n  operationId:\
  \ deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/extend\n  method: post\n  operationId: extendQosSessionDuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-sessions\n  method: post\n  operationId: retrieveSessionsByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - quality-on-demand:sessions:retrieve-by-device\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-date\n  method: post\n  operationId: retrieveSimSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap\n    - sim-swap:retrieve-date\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: checkSimSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap\n    - sim-swap:check\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n\
  \  method: post\n  operationId: createSimSwapSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap-subscriptions:org.camaraproject.sim-swap-subscriptions.v0.swapped:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: retrieveSubscriptionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sim-swap-subscriptions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}\n  method: get\n  operationId: retrieveSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sim-swap-subscriptions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap-subscriptions:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve-closest-edge-cloud-zone\n  method: post\n  operationId: readClosestEdgeCloudZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - simple-edge-discovery:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /short-message\n  method: post\n  operationId: send-sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - send-sms:short-message\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camara-project/refs/heads/main/agentic-access/camara-project-agentic-access.yml
summary_line: 49 operations · 39 acting · 1 human-in-the-loop
tags:
- API Standards
- CAMARA
- GSMA
- Linux Foundation
- Network APIs
- Open API
- Open Gateway
- Open Source
- Standards
- Telco
- Telco API Alliance
- Telecom
- Telecommunications
---
