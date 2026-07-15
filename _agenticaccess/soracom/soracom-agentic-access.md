---
acting_count: 616
action_class_counts:
  acting: 616
  connected: 344
api_specs:
- filename: soracom-sim-api-openapi.yml
  format: yaml
  label: Soracom SIM Management API
  slug: soracom-sim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-sim-api-openapi.yml
- filename: soracom-group-api-openapi.yml
  format: yaml
  label: Soracom Group Configuration API
  slug: soracom-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-group-api-openapi.yml
- filename: soracom-harvest-api-openapi.yml
  format: yaml
  label: Soracom Harvest API
  slug: soracom-harvest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-harvest-api-openapi.yml
- filename: soracom-inventory-api-openapi.yml
  format: yaml
  label: Soracom Inventory API
  slug: soracom-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-inventory-api-openapi.yml
- filename: soracom-napter-api-openapi.yml
  format: yaml
  label: Soracom Napter API
  slug: soracom-napter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-napter-api-openapi.yml
- filename: soracom-event-handler-api-openapi.yml
  format: yaml
  label: Soracom Event Handler API
  slug: soracom-event-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-event-handler-api-openapi.yml
- filename: soracom-vpg-api-openapi.yml
  format: yaml
  label: Soracom Virtual Private Gateway API
  slug: soracom-vpg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-vpg-api-openapi.yml
- filename: soracom-billing-api-openapi.yml
  format: yaml
  label: Soracom Billing API
  slug: soracom-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-billing-api-openapi.yml
- filename: soracom-stats-api-openapi.yml
  format: yaml
  label: Soracom Stats and Diagnostics API
  slug: soracom-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-stats-api-openapi.yml
- filename: soracom-auth-api-openapi.yml
  format: yaml
  label: Soracom Auth and Access Management API
  slug: soracom-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-auth-api-openapi.yml
- filename: soracom-analysis-query-api-openapi.yml
  format: yaml
  label: Soracom Analysis and Query API
  slug: soracom-analysis-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-analysis-query-api-openapi.yml
- filename: soracom-lagoon-api-openapi.yml
  format: yaml
  label: Soracom Lagoon API
  slug: soracom-lagoon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-lagoon-api-openapi.yml
- filename: soracom-lorawan-api-openapi.yml
  format: yaml
  label: Soracom Air for LoRaWAN API
  slug: soracom-lorawan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-lorawan-api-openapi.yml
- filename: soracom-sigfox-api-openapi.yml
  format: yaml
  label: Soracom Air for Sigfox API
  slug: soracom-sigfox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-sigfox-api-openapi.yml
- filename: soracom-soracam-api-openapi.yml
  format: yaml
  label: Soracom Cloud Camera Services API
  slug: soracom-soracam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-soracam-api-openapi.yml
- filename: soracom-batch-api-openapi.yml
  format: yaml
  label: Soracom Batch API
  slug: soracom-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-batch-api-openapi.yml
- filename: soracom-platform-api-openapi.yml
  format: yaml
  label: Soracom Platform API (Aggregate)
  slug: soracom-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-platform-api-openapi.yml
- filename: soracom-sandbox-api-openapi.yml
  format: yaml
  label: Soracom Sandbox API
  slug: soracom-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-sandbox-api-openapi.yml
consequence_counts:
  physical: 71
  read: 344
  safety-critical: 72
  write: 473
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 72
kind: agentic-access
layout: agentic-access
method: generated
name: Soracom Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/password_reset_token/issue
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/password_reset_token/issue
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/password_reset_token/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/password_reset_token/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/{device_id}/{object}/{instance}/unobserve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/{device_id}/{object}/{instance}/unobserve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/{device_id}/{object}/{instance}/{resource}/unobserve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/{device_id}/{object}/{instance}/{resource}/unobserve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gadgets/{product_id}/{serial_number}/disable_termination
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gadgets/{product_id}/{serial_number}/disable_termination
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gadgets/{product_id}/{serial_number}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gadgets/{product_id}/{serial_number}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lagoon/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lagoon/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_devices/{device_id}/disable_termination
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_devices/{device_id}/disable_termination
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_devices/{device_id}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_devices/{device_id}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_gateways/{gateway_id}/disable_termination
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_gateways/{gateway_id}/disable_termination
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_gateways/{gateway_id}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_gateways/{gateway_id}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lora_network_sets/{ns_id}/revoke_permission
operation_count: 960
overview: 'Soracom exposes 960 API operations that an AI agent could call, of which 616 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 344 read, 473 write, 71 physical, and 72 safety-critical.


  72 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Soracom
provider_slug: soracom
slug: soracom-agentic-access
source_filename: soracom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/soracom-analysis-query-api-openapi.yml, openapi/soracom-auth-api-openapi.yml,\n  openapi/soracom-batch-api-openapi.yml, openapi/soracom-billing-api-openapi.yml, openapi/soracom-event-handler-api-openapi.yml,\n  openapi/soracom-group-api-openapi.yml, openapi/soracom-harvest-api-openapi.yml, openapi/soracom-inventory-api-openapi.yml,\n  openapi/soracom-lagoon-api-openapi.yml, openapi/soracom-lorawan-api-openapi.yml, openapi/soracom-napter-api-openapi.yml,\n  openapi/soracom-platform-api-openapi.yml, openapi/soracom-sandbox-api-openapi.yml, openapi/soracom-sigfox-api-openapi.yml,\n  openapi/soracom-sim-api-openapi.yml, openapi/soracom-soracam-api-openapi.yml, openapi/soracom-stats-api-openapi.yml,\n  openapi/soracom-vpg-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and\
  \ bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 960\n  by_action_class:\n    acting: 616\n    connected: 344\n  by_consequence:\n    write: 473\n    read: 344\n    safety-critical: 72\n    physical: 71\n  human_in_the_loop_required: 72\noperations:\n- path: /analysis/queries\n  method: post\n  operationId: startAnalysisQueries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/queries/{query_id}\n  method: get\n  operationId: getAnalysisQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/schemas\n  method: get\n  operationId: getAnalysisSchemas\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/devices\n  method: get\n  operationId: searchDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/sigfox_devices\n  method: get\n  operationId: searchSigfoxDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/sims\n  method: get\n  operationId: searchSims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/subscribers\n  method: get\n  operationId: searchSubscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/subscribers/traffic_volume/ranking\n\
  \  method: get\n  operationId: searchSubscriberTrafficVolumeRanking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource_summaries/{resource_summary_type}\n  method: get\n  operationId: getResourceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth\n  method: post\n  operationId: auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/password_reset_token/issue\n  method: post\n  operationId: issuePasswordResetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/password_reset_token/verify\n  method: post\n  operationId: verifyPasswordResetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/switch_user\n\
  \  method: post\n  operationId: switchUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}\n  method: get\n  operationId: getOperator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/auth_keys\n  method: get\n  operationId: listOperatorAuthKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/auth_keys\n  method: post\n  operationId: generateOperatorAuthKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/auth_keys/{auth_key_id}\n  method: delete\n  operationId: deleteOperatorAuthKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/company_information\n  method: get\n  operationId: getCompanyInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/company_information\n  method: post\n  operationId: createCompanyInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/company_information\n  method: put\n  operationId: updateCompanyInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/configuration/{namespace}\n  method: delete\n  operationId: deleteOperatorConfigurationNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/configuration/{namespace}\n\
  \  method: get\n  operationId: getOperatorConfigurationNamespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/configuration/{namespace}\n  method: post\n  operationId: setOperatorConfigurationNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/contracts\n  method: post\n  operationId: addOperatorContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/contracts/{contract_name}\n\
  \  method: delete\n  operationId: deleteOperatorContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/coverage_type/{coverage_type}\n  method: post\n  operationId: addCoverageType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/individual_information\n  method: get\n  operationId: getIndividualInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/individual_information\n\
  \  method: post\n  operationId: createIndividualInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/individual_information\n  method: put\n  operationId: updateIndividualInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/mfa\n  method: delete\n  operationId: revokeMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /operators/{operator_id}/mfa\n  method: get\n  operationId: getMFAStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/mfa\n  method: post\n  operationId: enableMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/mfa/verify\n  method: post\n  operationId: verifyMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/password\n  method: post\n  operationId: updateOperatorPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/support/token\n  method: post\n  operationId: generateSupportToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/token\n  method: post\n  operationId: generateAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/tokens\n  method: delete\n  operationId: revokeOperatorAuthTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /operators/mfa_revoke_token/issue\n  method: post\n  operationId: issueMFARevokingToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /operators/mfa_revoke_token/verify\n  method: post\n  operationId: verifyMFARevokingToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /operators/{operator_id}/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /operators/{operator_id}/users/{user_name}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /operators/{operator_id}/users/{user_name}/auth_keys\n  method: get\n  operationId: listUserAuthKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/auth_keys\n  method: post\n  operationId: generateUserAuthKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/auth_keys/{auth_key_id}\n  method: delete\n  operationId: deleteUserAuthKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/auth_keys/{auth_key_id}\n  method: get\n  operationId: getUserAuthKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/mfa\n  method: delete\n  operationId: revokeUserMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/mfa\n  method: get\n  operationId: getUserMFAStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/mfa\n\
  \  method: post\n  operationId: enableUserMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/mfa/verify\n  method: post\n  operationId: verifyUserMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/password\n  method: delete\n  operationId: deleteUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/password\n  method: get\n  operationId: hasUserPassword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/password\n  method: post\n  operationId: createUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/password\n  method: put\n  operationId: updateUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/permission\n  method: delete\n  operationId: deleteUserPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/permission\n  method: get\n  operationId: getUserPermission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/permission\n  method: put\n  operationId: updateUserPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/tokens\n  method: delete\n  operationId: revokeUserAuthTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/trust_policy\n  method: delete\n  operationId: deleteUserTrustPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/trust_policy\n\
  \  method: get\n  operationId: getUserTrustPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/trust_policy\n  method: put\n  operationId: updateUserTrustPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/default_permissions\n  method: delete\n  operationId: deleteDefaultPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/default_permissions\n\
  \  method: get\n  operationId: getDefaultPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/default_permissions\n  method: put\n  operationId: updateDefaultPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/roles/{role_id}\n  method: delete\n  operationId: deleteRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/roles/{role_id}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/roles/{role_id}\n  method: post\n  operationId: createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/roles/{role_id}\n  method: put\n  operationId: updateRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/roles/{role_id}/users\n  method: get\n  operationId: listRoleAttachedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/roles/{role_id}/versions\n  method: get\n  operationId: listRoleVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/roles\n  method: get\n  operationId: listUserRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/users/{user_name}/roles\n  method: post\n  operationId: attachRole\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/users/{user_name}/roles/{role_id}\n  method: delete\n  operationId: detachRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/emails\n  method: get\n  operationId: listEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/emails/{email_id}\n  method: delete\n  operationId: deleteEmail\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/emails/{email_id}\n  method: get\n  operationId: getEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/add_email_token/issue\n  method: post\n  operationId: issueAddEmailToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/add_email_token/verify\n  method: post\n  operationId: verifyAddEmailToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/system_notifications\n  method: get\n  operationId: listSystemNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/system_notifications/{type}\n  method: delete\n  operationId: deleteSystemNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operator_id}/system_notifications/{type}\n  method: get\n  operationId: getSystemNotification\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_id}/system_notifications/{type}\n  method: post\n  operationId: setSystemNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch_groups\n  method: get\n  operationId: listBatchGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch_groups\n  method: post\n  operationId: createBatchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch_groups/{batch_group_id}\n  method: delete\n  operationId: deleteBatchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch_groups/{batch_group_id}\n  method: get\n  operationId: getBatchGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch_groups/{batch_group_id}\n  method: put\n  operationId: updateBatchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /batch_groups/{batch_group_id}/jobs\n  method: get\n  operationId: listBatchJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch_groups/{batch_group_id}/jobs\n  method: post\n  operationId: createBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch_groups/{batch_group_id}/jobs/{job_id}\n  method: get\n  operationId: getBatchJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch_groups/{batch_group_id}/jobs/{job_id}/tasks\n  method: get\n  operationId: listTasksOfBatchJob\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills\n  method: get\n  operationId: getBillingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{yyyyMM}\n  method: get\n  operationId: getBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{yyyyMM}/daily\n  method: get\n  operationId: getBillingPerDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{yyyyMM}/export\n  method: post\n  operationId: exportBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/latest\n  method: get\n  operationId: getLatestBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/latest/export\n  method: post\n  operationId: exportLatestBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\n\n# --- truncated at 32 KB (304 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/agentic-access/soracom-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/agentic-access/soracom-agentic-access.yml
summary_line: 960 operations · 616 acting · 72 human-in-the-loop
tags:
- IoT
- Cellular
- LPWAN
- SIM
- LoRaWAN
- Sigfox
- MVNO
- Connectivity
- Edge
- Japan
---
