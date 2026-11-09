---
acting_count: 84
action_class_counts:
  acting: 84
  connected: 81
api_specs:
- filename: skavio-eu-batch-processing-api-openapi.yml
  format: yaml
  label: skavio-eu Batch processing API
  slug: skavio-eu-batch-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-batch-processing-api-openapi.yml
- filename: skavio-eu-billing-api-openapi.yml
  format: yaml
  label: skavio-eu Billing API
  slug: skavio-eu-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-billing-api-openapi.yml
- filename: skavio-eu-bulk-manifests-api-openapi.yml
  format: yaml
  label: skavio-eu Bulk manifests API
  slug: skavio-eu-bulk-manifests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-bulk-manifests-api-openapi.yml
- filename: skavio-eu-contacts-api-openapi.yml
  format: yaml
  label: skavio-eu Contacts API
  slug: skavio-eu-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-contacts-api-openapi.yml
- filename: skavio-eu-events-api-openapi.yml
  format: yaml
  label: skavio-eu Events API
  slug: skavio-eu-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-events-api-openapi.yml
- filename: skavio-eu-flow-api-openapi.yml
  format: yaml
  label: skavio-eu Flow API
  slug: skavio-eu-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-flow-api-openapi.yml
- filename: skavio-eu-invoices-api-openapi.yml
  format: yaml
  label: skavio-eu Invoices API
  slug: skavio-eu-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-invoices-api-openapi.yml
- filename: skavio-eu-me-api-openapi.yml
  format: yaml
  label: skavio-eu Me API
  slug: skavio-eu-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-me-api-openapi.yml
- filename: skavio-eu-operational-notifications-api-openapi.yml
  format: yaml
  label: skavio-eu Operational notifications API
  slug: skavio-eu-operational-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-operational-notifications-api-openapi.yml
- filename: skavio-eu-paid-web-data-api-openapi.yml
  format: yaml
  label: skavio-eu paid web data API
  slug: skavio-eu-paid-web-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-paid-web-data-api-openapi.yml
- filename: skavio-eu-requests-api-openapi.yml
  format: yaml
  label: skavio-eu Requests API
  slug: skavio-eu-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-requests-api-openapi.yml
- filename: skavio-eu-skavio-accounting-api-openapi.yml
  format: yaml
  label: skavio-eu Skavio Accounting API
  slug: skavio-eu-skavio-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-skavio-accounting-api-openapi.yml
- filename: skavio-eu-skavio-processing-api-api-openapi.yml
  format: yaml
  label: skavio-eu Skavio processing API
  slug: skavio-eu-skavio-processing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-skavio-processing-api-api-openapi.yml
- filename: skavio-eu-usdc-payment-verification-api-openapi.yml
  format: yaml
  label: skavio-eu USDC payment verification API
  slug: skavio-eu-usdc-payment-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-usdc-payment-verification-api-openapi.yml
- filename: skavio-eu-webhooks-api-openapi.yml
  format: yaml
  label: skavio-eu Webhooks API
  slug: skavio-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-webhooks-api-openapi.yml
- filename: skavio-eu-workflow-pipelines-api-openapi.yml
  format: yaml
  label: skavio-eu Workflow pipelines API
  slug: skavio-eu-workflow-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-workflow-pipelines-api-openapi.yml
- filename: skavio-eu-x402-api-openapi.yml
  format: yaml
  label: skavio-eu X402 API
  slug: skavio-eu-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-x402-api-openapi.yml
consequence_counts:
  physical: 11
  read: 81
  safety-critical: 18
  write: 55
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Skavio Eu Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/accounting/connections/{connection_id}/disconnect
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/bulks/{bulk_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulks/{bulk_id}/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulks/{bulk_id}/pause
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulks/{bulk_id}/retry-failed
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulks/{bulk_id}/seal
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/pipelines/{pipeline_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/webhooks/{webhook_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/workflow-runs/{run_id}/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /x402/v1/processing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /x402/v1/processing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /x402/v1/processing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /x402/v1/processing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /x402/v1/processing/{operation}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /x402/v1/processing/{operation}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /x402/v1/processing/{operation}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /x402/v1/processing/{operation}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/drafts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/personal/requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/subscribe
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/subscription/confirm
operation_count: 165
overview: 'skavio-eu exposes 165 API operations that an AI agent could call, of which 84 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 81 read, 55 write, 11 physical, and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: skavio-eu
provider_slug: skavio-eu
slug: skavio-eu-agentic-access
source_filename: skavio-eu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/skavio-eu-processing-openapi.json, openapi/skavio-eu-proof-openapi.json, openapi/skavio-eu-x402-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 165\n  by_action_class:\n    acting: 84\n    connected: 81\n  by_consequence:\n    write: 55\n    read: 81\n    safety-critical: 18\n    physical: 11\n  human_in_the_loop_required: 18\noperations:\n- path: /v1/batches/estimate\n  method: post\n  operationId: estimate_batch_v1_batches_estimate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/batches\n  method: post\n  operationId: submit_batch_v1_batches_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches\n  method: get\n  operationId: batches_v1_batches_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/{batch_id}\n  method: get\n  operationId: batch_v1_batches__batch_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/{batch_id}\n  method: delete\n  operationId: delete_batch_v1_batches__batch_id__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/{batch_id}/results.zip\n  method: get\n  operationId: batch_zip_v1_batches__batch_id__results_zip_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/{batch_id}/retry-failed\n  method: post\n  operationId: retry_failed_v1_batches__batch_id__retry_failed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulks\n  method: post\n  operationId: create_v1_bulks_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulks\n  method: get\n  operationId: listing_v1_bulks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulks/{bulk_id}/manifest\n  method: put\n  operationId: append_v1_bulks__bulk_id__manifest_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulks/{bulk_id}/seal\n  method: post\n  operationId: seal_v1_bulks__bulk_id__seal_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulks/{bulk_id}\n  method: get\n  operationId: status_v1_bulks__bulk_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulks/{bulk_id}\n  method: delete\n  operationId: cancel_v1_bulks__bulk_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulks/{bulk_id}/items\n  method: get\n  operationId: items_v1_bulks__bulk_id__items_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulks/{bulk_id}/outputs\n  method: get\n  operationId: outputs_v1_bulks__bulk_id__outputs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulks/{bulk_id}/pause\n  method: post\n  operationId: pause_control_v1_bulks__bulk_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulks/{bulk_id}/cancel\n  method: post\n  operationId: cancel_control_v1_bulks__bulk_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulks/{bulk_id}/resume\n  method: post\n  operationId: resume_v1_bulks__bulk_id__resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulks/{bulk_id}/retry-failed\n  method: post\n  operationId: retry_v1_bulks__bulk_id__retry_failed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/pipelines\n  method: get\n  operationId: list_pipelines_v1_pipelines_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pipelines\n  method: post\n  operationId: create_pipeline_v1_pipelines_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pipelines/{pipeline_id}\n  method: delete\n  operationId: delete_pipeline_v1_pipelines__pipeline_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workflow-runs\n  method: post\n  operationId: create_run_v1_workflow_runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflow-runs\n  method: get\n  operationId: list_runs_v1_workflow_runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflow-runs/{run_id}\n  method: get\n  operationId: get_run_v1_workflow_runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflow-runs/{run_id}/pause\n  method: post\n  operationId:\
  \ pause_v1_workflow_runs__run_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflow-runs/{run_id}/cancel\n  method: post\n  operationId: cancel_v1_workflow_runs__run_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workflow-runs/{run_id}/resume\n  method: post\n  operationId: resume_v1_workflow_runs__run_id__resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflow-runs/{run_id}/approve\n  method: post\n  operationId: approve_v1_workflow_runs__run_id__approve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/settings\n  method: get\n  operationId: settings_v1_notifications_settings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/settings\n  method: put\n  operationId: update_v1_notifications_settings_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications\n  method: get\n  operationId: listing_v1_notifications_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pricing\n  method: get\n  operationId: public_pricing_v1_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities\n  method: get\n  operationId: capabilities_v1_capabilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage\n  method: get\n  operationId: storage_status_v1_storage_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet\n  method: get\n  operationId: wallet_v1_wallet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: get\n  operationId: keys_v1_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: new_key_v1_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{key_id}\n  method: delete\n  operationId: revoke_v1_keys__key_id__delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/uploads\n  method: post\n  operationId: uploads_v1_uploads_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{upload_id}\n  method: delete\n  operationId: delete_upload_v1_uploads__upload_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /v1/estimate\n  method: post\n  operationId: estimate_v1_estimate_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  operationId: submit_v1_jobs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: jobs_v1_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: job_v1_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: delete\n  operationId: delete_job_v1_jobs__job_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}/results/{result_id}\n  method: get\n  operationId: result_v1_jobs__job_id__results__result_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows\n  method: get\n  operationId: workflows_v1_workflows_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows\n  method: post\n  operationId: save_workflow_v1_workflows_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflow_id}\n  method: delete\n  operationId: delete_workflow_v1_workflows__workflow_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout\n  method: post\n  operationId: checkout_v1_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/confirm\n  method: post\n  operationId: confirm_v1_billing_confirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/usage\n  method: get\n  operationId: storage_usage_v1_storage_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/policy\n  method: get\n  operationId: get_storage_policy_v1_storage_policy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/storage/policy\n  method: patch\n  operationId: patch_storage_policy_v1_storage_policy_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/direct-uploads\n  method: post\n  operationId: direct_upload_v1_storage_direct_uploads_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/direct-uploads/{session_id}/complete\n  method: post\n  operationId: complete_direct_v1_storage_direct_uploads__session_id__complete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/imports\n  method: post\n  operationId: cloud_import_v1_storage_imports_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/imports/{import_id}\n  method: get\n  operationId: import_status_v1_storage_imports__import_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/objects\n  method: get\n  operationId: objects_v1_storage_objects_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/objects/{object_id}\n  method: get\n  operationId: object_status_v1_storage_objects__object_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/objects/{object_id}\n  method: delete\n  operationId: object_delete_v1_storage_objects__object_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/objects/{object_id}/download-link\n  method: get\n  operationId: object_download_v1_storage_objects__object_id__download_link_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/objects/{object_id}/backup\n  method: post\n  operationId: object_backup_v1_storage_objects__object_id__backup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/objects/{object_id}/restore-backup\n  method: post\n  operationId: object_restore_backup_v1_storage_objects__object_id__restore_backup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/objects/{object_id}/archive\n  method: post\n  operationId: object_archive_v1_storage_objects__object_id__archive_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/objects/{object_id}/restore\n  method: post\n  operationId: object_restore_v1_storage_objects__object_id__restore_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/objects/{object_id}/hold\n  method: post\n  operationId: object_hold_v1_storage_objects__object_id__hold_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/audit\n  method: get\n  operationId: storage_audit_v1_storage_audit_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/jobs\n  method: get\n  operationId: history_v1_usage_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/payments\n  method: get\n  operationId: payments_v1_usage_payments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/usage/export.csv\n  method: get\n  operationId: export_v1_usage_export_csv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/budgets\n  method: get\n  operationId: budgets_v1_budgets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/budgets\n  method: put\n  operationId: set_budget_v1_budgets_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts\n  method: get\n  operationId: alerts_v1_alerts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/keys/{key_id}/policy\n  method: put\n  operationId: key_policy_v1_keys__key_id__policy_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{key_id}/policy\n  method: get\n  operationId: get_key_policy_v1_keys__key_id__policy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/governance/audit\n  method: get\n  operationId: audit_v1_governance_audit_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_v1_jobs__job_id__cancel_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/operations\n  method: get\n  operationId: operations_v1_operations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/context\n  method: get\n  operationId: context_v1_maya_context_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/messages\n  method: post\n  operationId: message_v1_maya_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/editorial-status\n  method: get\n  operationId: editorial_status_v1_maya_editorial_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/seo-status\n  method: get\n  operationId: seo_status_v1_maya_seo_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/public-chat\n  method: post\n  operationId: public_chat_v1_maya_public_chat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/tickets\n\
  \  method: get\n  operationId: list_customer_v1_maya_support_tickets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/support/tickets\n  method: post\n  operationId: create_v1_maya_support_tickets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/owner/tickets\n  method: get\n  operationId: list_owner_v1_maya_support_owner_tickets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/support/tickets/{tid}\n  method: get\n  operationId: customer_detail_v1_maya_support_tickets__tid__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/support/owner/tickets/{tid}\n  method: get\n  operationId: owner_detail_v1_maya_support_owner_tickets__tid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maya/support/owner/tickets/{tid}\n  method: patch\n  operationId: status_v1_maya_support_owner_tickets__tid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/tickets/{tid}/messages\n  method: post\n  operationId: customer_comment_v1_maya_support_tickets__tid__messages_post\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/owner/tickets/{tid}/messages\n  method: post\n  operationId: owner_comment_v1_maya_support_owner_tickets__tid__messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/owner/tickets/{tid}/handoff\n  method: post\n  operationId: prepare_v1_maya_support_owner_tickets__tid__handoff_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/owner/tickets/{tid}/handoff/approve\n  method: post\n  operationId: approve_v1_maya_support_owner_tickets__tid__handoff_approve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maya/support/owner/tickets/{tid}/handoff/analyze\n  method: post\n  operationId: owner_codex_analysis_v1_maya_support_owner_tickets__tid__handoff_analyze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/deliveries\n  method:\
  \ get\n  operationId: deliveries_v1_webhooks_deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/deliveries/{kind}/{delivery_id}/replay\n  method: post\n  operationId: replay_v1_webhooks_deliveries__kind___delivery_id__replay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: webhooks_v1_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: create_v1_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}\n  method: delete\n  operationId: delete_v1_webhooks__webhook_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/billing/plans\n  method: get\n  operationId: plans_v1_billing_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (50 KB total) ---\n# Full source: https://artifacts.apis.io/skavio-eu/agentic-access/skavio-eu-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/skavio-eu/agentic-access/skavio-eu-agentic-access.yml
summary_line: 165 operations · 84 acting · 18 human-in-the-loop
tags:
- BusinessTools
- Document Processing
- Invoice Automation
- Audio Transcription
- Payments
---
