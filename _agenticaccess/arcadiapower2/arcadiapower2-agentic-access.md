---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 21
api_specs:
- filename: arcadiapower2-auth-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Auth API
  slug: arcadiapower2-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-auth-api-openapi.yml
- filename: arcadiapower2-bundle-beta-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Bundle (Beta) API
  slug: arcadiapower2-bundle-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-bundle-beta-api-openapi.yml
- filename: arcadiapower2-bundle-webhook-events-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Bundle Webhook Events API
  slug: arcadiapower2-bundle-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-bundle-webhook-events-api-openapi.yml
- filename: arcadiapower2-plug-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Plug API
  slug: arcadiapower2-plug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-plug-api-openapi.yml
- filename: arcadiapower2-spark-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Spark API
  slug: arcadiapower2-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-spark-api-openapi.yml
- filename: arcadiapower2-users-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Users API
  slug: arcadiapower2-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-users-api-openapi.yml
- filename: arcadiapower2-utility-accounts-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Accounts API
  slug: arcadiapower2-utility-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-accounts-api-openapi.yml
- filename: arcadiapower2-utility-credentials-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Credentials API
  slug: arcadiapower2-utility-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-credentials-api-openapi.yml
- filename: arcadiapower2-utility-meters-beta-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Meters (Beta) API
  slug: arcadiapower2-utility-meters-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-meters-beta-api-openapi.yml
- filename: arcadiapower2-webhook-events-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Webhook Events API
  slug: arcadiapower2-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-webhook-events-api-openapi.yml
- filename: arcadiapower2-webhooks-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Webhooks API
  slug: arcadiapower2-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 21
  safety-critical: 2
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Arcadiapower2 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sandbox/webhook/trigger/utility_credential_revoked
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /spark/storage_optimization/schedules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spark/charge_curve/cost
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spark/charge_curve/schedule
operation_count: 42
overview: 'Arcadiapower2 exposes 42 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 17 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Arcadiapower2
provider_slug: arcadiapower2
slug: arcadiapower2-agentic-access
source_filename: arcadiapower2-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/arcadiapower2-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 21\n    connected: 21\n  by_consequence:\n    write: 17\n    read: 21\n    physical: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /auth/access_token\n  method: post\n  operationId: createApiAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/connect_token\n  method: post\n  operationId: createConnectToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/connect_url\n  method: post\n  operationId: createConnectUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utility_accounts\n  method: get\n  operationId: getUtilityAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /utility_accounts/{utility_account_id}\n  method: get\n  operationId: getUtilityAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{client_user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{client_user_id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /utility_credentials\n  method: get\n  operationId: getUtilityCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utility_credentials/{utility_credential_id}\n  method: get\n  operationId: getUtilityCredential\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utility_meters\n  method: get\n  operationId: getUtilityMeters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utility_meters/{utility_meter_id}\n  method: get\n  operationId: getUtilityMeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /plug/utility_statements\n  method: get\n  operationId: getUtilityStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plug/utility_statements/{utility_statement_id}\n  method: get\n  operationId: getUtilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spark/charge_curve/cost\n  method: post\n  operationId: calculateChargeCost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spark/charge_curve/schedule\n  method: post\n  operationId: calculateSmartChargeSchedule\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spark/tariff_rates\n  method: post\n  operationId: retrieveTariffRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spark/optimized_tariffs/load_serving_entities\n  method: get\n  operationId: searchLoadServingEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spark/optimized_tariffs/applicabilities\n  method: get\n  operationId: getOptimizedTariffsApplicabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spark/optimized_tariffs/recommendations\n  method: post\n  operationId: searchOptimizedTariffsByApplicabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spark/optimized_tariffs/scenario_cost\n  method: post\n  operationId: calculateOptimizedTariffsScenarioCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spark/storage_optimization/schedules\n  method: post\n  operationId: calculateStorageOptimizationSchedules\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n \
  \     exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bundle/utility_remittance/utility_credentials/{utility_credential_id}/enroll\n  method: post\n  operationId: enrollUtilityRemittance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundle/utility_remittance/utility_credentials/{utility_credential_id}/remove\n  method: delete\n  operationId: removeUtilityRemittance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /bundle/utility_remittance/utility_statements/{utility_statement_id}/utility_remittance_items\n  method: post\n  operationId: createUtilityRemittanceItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundle/utility_remittance/utility_remittance_items/{utility_remittance_item_id}\n  method: get\n  operationId: getUtilityRemittanceItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundle/utility_remittance/utility_account/{utility_account_id}/enrollment\n  method: get\n  operationId: showUtilityRemittanceEnrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /webhook/endpoints\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/endpoints\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/endpoints/{webhook_endpoint_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/endpoints/{webhook_endpoint_id}\n\
  \  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/endpoints/{webhook_endpoint_id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/endpoints/{webhook_endpoint_id}/test\n  method: put\n  operationId: requestWebookTestEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/endpoints/{webhook_endpoint_id}/events\n\
  \  method: get\n  operationId: getWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/endpoints/{webhook_endpoint_id}/events/{webhook_event_id}\n  method: get\n  operationId: getWebhookEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/bundle/utility_remittance/utility_credentials/{utility_credential_id}/accept\n  method: post\n  operationId: sandboxUtilityRemittanceAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/bundle/utility_remittance/utility_credentials/{utility_credential_id}/reject\n  method:\
  \ post\n  operationId: sandboxUtilityRemittanceReject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/bundle/utility_remittance/utility_credentials/{utility_credential_id}/remove\n  method: post\n  operationId: sandboxUtilityRemittanceRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/connect/submit_test_credentials\n  method: post\n  operationId: submitTestCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/webhook/trigger/new_utility_statement_available\n  method: post\n  operationId: triggerNewUtilityStatementAvailable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/webhook/trigger/utility_credential_revoked\n  method: post\n  operationId: triggerUtilityCredentialRevoked\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/agentic-access/arcadiapower2-agentic-access.yml
summary_line: 42 operations · 21 acting · 2 human-in-the-loop
tags:
- Energy
- SaaS
- Enterprise
- Sustainability
- Data
---
