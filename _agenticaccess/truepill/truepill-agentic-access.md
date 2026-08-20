---
acting_count: 69
action_class_counts:
  acting: 69
  connected: 89
api_specs:
- filename: truepill-insurance-api-openapi.yml
  format: yaml
  label: Truepill Insurance API
  slug: truepill-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-insurance-api-openapi.yml
- filename: truepill-patients-api-openapi.yml
  format: yaml
  label: Truepill Patients API
  slug: truepill-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-patients-api-openapi.yml
- filename: truepill-prescriptions-api-openapi.yml
  format: yaml
  label: Truepill Prescriptions API
  slug: truepill-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-prescriptions-api-openapi.yml
- filename: truepill-transfers-api-openapi.yml
  format: yaml
  label: Truepill Transfers API
  slug: truepill-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-transfers-api-openapi.yml
- filename: truepill-webhooks-api-openapi.yml
  format: yaml
  label: Truepill Webhooks API
  slug: truepill-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-webhooks-api-openapi.yml
- filename: truepill-fulfillment-api-openapi.yml
  format: yaml
  label: Truepill Fulfillment API
  slug: truepill-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-fulfillment-api-openapi.yml
- filename: truepill-consults-api-openapi.yml
  format: yaml
  label: Truepill Consults API
  slug: truepill-consults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-consults-api-openapi.yml
- filename: truepill-diagnostics-api-openapi.yml
  format: yaml
  label: Truepill Diagnostics API
  slug: truepill-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-diagnostics-api-openapi.yml
- filename: truepill-media-api-openapi.yml
  format: yaml
  label: Truepill Media API
  slug: truepill-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-media-api-openapi.yml
consequence_counts:
  physical: 37
  read: 89
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Truepill Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/auto-refill/{prescription_token}/early-refill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cancel_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/direct_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external_location_matches
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/fill_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/fill_request/{url_token}/stripe_payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/fuzion_test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/prescriber
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/prescription/{prescription_token}/external_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/prescription/{prescription_token}/transfer_out
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/prescriptions/{prescription_token}/external_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/same_day_delivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfer_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/update_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/direct_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /diagnostics/v0/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /diagnostics/v0/orders/register
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scheduled-fill-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /scheduled-fill-requests/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /scheduled-fill-requests/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auto-refill/{prescription_token}/early-refill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cancel_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/direct_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_location_matches
operation_count: 158
overview: 'Truepill exposes 158 API operations that an AI agent could call, of which 69 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 89 read, 32 write, and 37 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Truepill
provider_slug: truepill
slug: truepill-agentic-access
source_filename: truepill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: generated\nsource: openapi/truepill-consults-api-openapi.yml, openapi/truepill-diagnostics-api-openapi.yml,\n  openapi/truepill-fulfillment-api-openapi.yml, openapi/truepill-insurance-api-openapi.yml,\n  openapi/truepill-media-api-openapi.yml, openapi/truepill-patients-api-openapi.yml, openapi/truepill-prescriptions-api-openapi.yml,\n  openapi/truepill-transfers-api-openapi.yml, openapi/truepill-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 158\n  by_action_class:\n    connected: 89\n    acting: 69\n  by_consequence:\n    read: 89\n    write: 32\n    physical: 37\n  human_in_the_loop_required: 0\noperations:\n- path: /consults/v0\n  method: get\n  operationId: getConsultsV0\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consults/v0/consult\n  method: post\n  operationId: postConsultsV0Consult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consults/v0/consult/{consult_id}\n  method: get\n  operationId: getConsultsV0ConsultConsult_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consults/v0/consult/{consult_id}\n  method: delete\n  operationId: deleteConsultsV0ConsultConsult_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consults/v0/consult/{consult_id}/media\n  method: patch\n  operationId: patchConsultsV0ConsultConsult_idMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consults/v0/consult/{consult_id}/simulate\n  method: patch\n  operationId: patchConsultsV0ConsultConsult_idSimulate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /diagnostics/v0/kits\n  method: get\n  operationId: getDiagnosticsV0Kits\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/v0/kits/{kit_id}/validation/kit_serial\n  method: get\n  operationId: getDiagnosticsV0KitsKit_idValidationKit_serial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/v0/orders\n  method: get\n  operationId: getDiagnosticsV0Orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/v0/orders\n  method: post\n  operationId: postDiagnosticsV0Orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /diagnostics/v0/orders/register\n  method: post\n  operationId: postDiagnosticsV0OrdersRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /diagnostics/v0/orders/{order_id}\n  method: get\n  operationId: getDiagnosticsV0OrdersOrder_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/v0/orders/{order_id}/rejection\n  method: get\n  operationId: getDiagnosticsV0OrdersOrder_idRejection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /diagnostics/v0/orders/{order_id}/results\n  method: get\n  operationId: getDiagnosticsV0OrdersOrder_idResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/v0/tests\n  method: get\n  operationId: getDiagnosticsV0Tests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/v2/orders/{order_id}/results\n  method: get\n  operationId: getDiagnosticsV2OrdersOrder_idResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/availability\n  method: get\n  operationId: getApiV1Availability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/cancel_request\n  method: post\n  operationId: postApiV1Cancel_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fill_request\n  method: post\n  operationId: postApiV1Fill_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fill_request/{url_token}\n  method: get\n  operationId: getApiV1Fill_requestUrl_token\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fill_request/{url_token}/stripe_payment\n  method: put\n  operationId: putApiV1Fill_requestUrl_tokenStripe_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fill_requests\n  method: get\n  operationId: getApiV1Fill_requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fuzion_test\n  method: post\n  operationId: postApiV1Fuzion_test\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/nearby_same_day_pickup_locations\n  method: get\n  operationId: getApiV1Nearby_same_day_pickup_locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/open-api/api.yml\n  method: get\n  operationId: getApiV1OpenapiApiyml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/order\n  method: post\n  operationId: postApiV1Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/order/{token}\n  method: get\n  operationId: getApiV1OrderToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prescriber\n  method: post\n  operationId: postApiV1Prescriber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prescriber/{prescriber_token}\n  method: get\n  operationId: getApiV1PrescriberPrescriber_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/same_day_delivery\n\
  \  method: get\n  operationId: getApiV1Same_day_delivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/same_day_delivery\n  method: post\n  operationId: postApiV1Same_day_delivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/same_day_delivery/{id}\n  method: get\n  operationId: getApiV1Same_day_deliveryId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/specialty_pharmacies\n  method: get\n  operationId: getApiV1Specialty_pharmacies\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/update_request\n  method: post\n  operationId: postApiV1Update_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled-actions\n  method: get\n  operationId: getScheduledactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-fill-requests\n  method: get\n  operationId: getScheduledfillrequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-fill-requests\n\
  \  method: post\n  operationId: postScheduledfillrequests\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled-fill-requests/{id}\n  method: put\n  operationId: putScheduledfillrequestsId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled-fill-requests/{id}\n  method: delete\n  operationId: deleteScheduledfillrequestsId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/schedule\n  method: get\n  operationId: getV0Schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/availability\n  method: get\n  operationId: getV1Availability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cancel_request\n  method: post\n  operationId: postV1Cancel_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fill_request\n  method: post\n  operationId: postV1Fill_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fill_request/{url_token}\n  method: get\n  operationId: getV1Fill_requestUrl_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fill_request/{url_token}/stripe_payment\n  method: put\n  operationId: putV1Fill_requestUrl_tokenStripe_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fill_requests\n  method: get\n  operationId: getV1Fill_requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fuzion_test\n  method: post\n  operationId: postV1Fuzion_test\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/nearby_same_day_pickup_locations\n  method: get\n  operationId: getV1Nearby_same_day_pickup_locations\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-api/api.yml\n  method: get\n  operationId: getV1OpenapiApiyml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order\n  method: post\n  operationId: postV1Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{token}\n  method: get\n  operationId: getV1OrderToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prescriber\n  method: post\n  operationId: postV1Prescriber\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prescriber/{prescriber_token}\n  method: get\n  operationId: getV1PrescriberPrescriber_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/same_day_delivery\n  method: get\n  operationId: getV1Same_day_delivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/same_day_delivery\n  method: post\n  operationId: postV1Same_day_delivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/same_day_delivery/{id}\n  method: get\n  operationId: getV1Same_day_deliveryId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specialty_pharmacies\n  method: get\n  operationId: getV1Specialty_pharmacies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/update_request\n  method: post\n  operationId: postV1Update_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/copay_request\n  method: post\n  operationId: postApiV1Copay_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/copay_request/cancel\n  method: post\n  operationId: postApiV1Copay_requestCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/copay_request/{request_id}\n  method: get\n  operationId: getApiV1Copay_requestRequest_id\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage_request\n  method: post\n  operationId: postApiV1Coverage_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance\n  method: post\n  operationId: postApiV1Insurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance/eligibility-check\n  method: post\n  operationId: postApiV1InsuranceEligibilitycheck\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance/{insurance_token}\n  method: get\n  operationId: getApiV1InsuranceInsurance_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pharmacy-coverage\n  method: get\n  operationId: getApiV1Pharmacycoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prior_authorization\n  method: post\n  operationId: postApiV1Prior_authorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copay_request\n  method: post\n  operationId: postV1Copay_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copay_request/cancel\n  method: post\n  operationId: postV1Copay_requestCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copay_request/{request_id}\n  method: get\n  operationId: getV1Copay_requestRequest_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverage_request\n  method: post\n  operationId: postV1Coverage_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insurance\n  method: post\n  operationId: postV1Insurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insurance/eligibility-check\n  method: post\n  operationId: postV1InsuranceEligibilitycheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insurance/{insurance_token}\n  method: get\n  operationId: getV1InsuranceInsurance_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pharmacy-coverage\n  method: get\n  operationId: getV1Pharmacycoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prior_authorization\n  method: post\n  operationId: postV1Prior_authorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/media\n\
  \  method: post\n  operationId: postApiV1Media\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/media/{id}\n  method: get\n  operationId: getApiV1MediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/media/{id}/signed-url/read\n  method: get\n  operationId: getApiV1MediaIdSignedurlRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/media/{id}/signed-url/write\n  method: get\n  operationId: getApiV1MediaIdSignedurlWrite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/media\n  method: post\n  operationId: postApiV2Media\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/media/{id}\n  method: get\n  operationId: getApiV2MediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media\n  method: post\n  operationId: postV1Media\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/{id}\n  method: get\n  operationId:\
  \ getV1MediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media/{id}/signed-url/read\n  method: get\n  operationId: getV1MediaIdSignedurlRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media/{id}/signed-url/write\n  method: get\n  operationId: getV1MediaIdSignedurlWrite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/media\n  method: post\n  operationId: postV2Media\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/media/{id}\n\
  \  method: get\n  operationId: getV2MediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patient\n  method: get\n  operationId: getApiV1Patient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patient\n  method: put\n  operationId: putApiV1Patient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patient/{patient_token}\n  method: get\n  operationId: getApiV1PatientPatient_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/patient/{patient_token}\n  method: post\n  operationId: postApiV1PatientPatient_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patient/{patient_token}/patient_survey\n  method: get\n  operationId: getApiV1PatientPatient_tokenPatient_survey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patient/{patient_token}/prescriptions\n  method: get\n  operationId: getApiV1PatientPatient_tokenPrescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patient\n  method: get\n  operationId: getV1Patient\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patient\n  method: put\n  operationId: putV1Patient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patient/{patient_token}\n  method: get\n  operationId: getV1PatientPatient_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patient/{patient_token}\n  method: post\n  operationId: postV1PatientPatient_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patient/{patient_token}/patient_survey\n  method: get\n  operationId: getV1PatientPatient_tokenPatient_survey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patient/{patient_token}/prescriptions\n  method: get\n  operationId: getV1PatientPatient_tokenPrescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auto-refill\n  method: get\n  operationId: getApiV1Autorefill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auto-refill/patient/{patient_token}\n  method: get\n  operationId: getApiV1AutorefillPatientPatient_token\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auto-refill/{prescription_token}\n  method: get\n  operationId: getApiV1AutorefillPrescription_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auto-refill/{prescription_token}\n  method: post\n  operationId: postApiV1AutorefillPrescription_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auto-refill/{prescription_token}\n  method: delete\n  operationId: deleteApiV1AutorefillPrescription_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auto-refill/{prescription_token}/early-refill\n  method: post\n  operationId: postApiV1AutorefillPrescription_tokenEarlyrefill\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auto-refill/{prescription_token}/skip-refill\n  method: delete\n  operationId: deleteApiV1AutorefillPrescription_tokenSkiprefill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ trigge\n\n# --- truncated at 32 KB (47 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/agentic-access/truepill-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/agentic-access/truepill-agentic-access.yml
summary_line: 158 operations · 69 acting
tags:
- Pharmacy
- Healthcare
- Prescription Fulfillment
- Telehealth
- Diagnostics
- Insurance
- Copay Adjudication
- Prior Authorization
- Electronic Prescribing
- Pharmacy Transfers
- Webhook
- HIPAA
---
