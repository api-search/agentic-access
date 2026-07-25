---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 11
api_specs:
- filename: genlogs-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Alerts API
  slug: genlogs-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-alerts-api-openapi.yml
- filename: genlogs-auth-api-openapi.yml
  format: yaml
  label: GenLogs auth API
  slug: genlogs-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-auth-api-openapi.yml
- filename: genlogs-carrier-api-openapi.yml
  format: yaml
  label: GenLogs Carrier API
  slug: genlogs-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-carrier-api-openapi.yml
- filename: genlogs-carrier-vetting-api-openapi.yml
  format: yaml
  label: GenLogs carrier-vetting API
  slug: genlogs-carrier-vetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-carrier-vetting-api-openapi.yml
- filename: genlogs-compliance-rules-api-openapi.yml
  format: yaml
  label: GenLogs Compliance Rules API
  slug: genlogs-compliance-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-compliance-rules-api-openapi.yml
- filename: genlogs-facilities-api-openapi.yml
  format: yaml
  label: GenLogs Facilities API
  slug: genlogs-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-facilities-api-openapi.yml
- filename: genlogs-mismatch-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Mismatch alerts API
  slug: genlogs-mismatch-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-mismatch-alerts-api-openapi.yml
- filename: genlogs-onboarded-carriers-api-openapi.yml
  format: yaml
  label: GenLogs Onboarded Carriers API
  slug: genlogs-onboarded-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-onboarded-carriers-api-openapi.yml
- filename: genlogs-shipper-api-openapi.yml
  format: yaml
  label: GenLogs Shipper API
  slug: genlogs-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-shipper-api-openapi.yml
- filename: genlogs-webhook-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Webhook Alerts API
  slug: genlogs-webhook-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-webhook-alerts-api-openapi.yml
consequence_counts:
  read: 11
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Genlogs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'GenLogs exposes 28 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GenLogs
provider_slug: genlogs
slug: genlogs-agentic-access
source_filename: genlogs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/genlogs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 17\n    connected: 11\n  by_consequence:\n    write: 17\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carrier/recommendations\n  method: get\n  operationId: getCarrierRecommendations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carrier/contacts\n  method: post\n  operationId: searchCarrierContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarded-carrier/contacts\n  method: post\n  operationId: createOnboardedCarrierContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarded-carrier/contacts\n  method: get\n  operationId: listOnboardedCarrierContacts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarded-carrier/contacts/{contact_id}\n  method: patch\n  operationId: updateOnboardedCarrierContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarded-carrier/contacts/{contact_id}\n  method: delete\n  operationId: deleteOnboardedCarrierContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarded-carrier/bulk/contacts\n  method: post\n  operationId: createOnboardedCarrierContactsBulk\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarded-carrier/bulk/contacts\n  method: delete\n  operationId: deleteOnboardedCarrierContactsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compliance-rules\n  method: get\n  operationId: listComplianceRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer-compliance-rules/{customer_rule_id}\n  method: patch\n  operationId: updateCustomerComplianceRule\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer-compliance-rules\n  method: get\n  operationId: listCustomerComplianceRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipper/lanes\n  method: get\n  operationId: getShipperLanes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facilities\n  method: get\n  operationId: getShipperFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facility/{facility_id}/network-map\n  method: get\n  operationId: getFacilityNetworkMap\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mismatch-observations\n  method: post\n  operationId: createMismatchObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mismatch-observations\n  method: get\n  operationId: listMismatchObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mismatch-observations/{observation_id}\n  method: patch\n  operationId: updateMismatchObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mismatch-observations/{observation_id}\n  method: delete\n  operationId: deleteMismatchObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/{alert_id}\n  method: patch\n  operationId: external_patch_alert_alerts__alert_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/webhook\n  method: post\n  operationId: create_webhook_alerts_webhook_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/webhook\n  method: get\n  operationId: list_webhooks_alerts_webhook_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/webhook/{webhook_id}\n  method: patch\n  operationId: update_webhook_alerts_webhook__webhook_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/webhook/{webhook_id}\n  method: delete\n  operationId: deleteAlertWebhook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/webhook/test\n  method: post\n  operationId: validate_webhook_endpoint_alerts_webhook_test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carrier/profile\n  method: get\n  operationId: getCarrierProfileDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token/refresh\n  method: post\n  operationId: refresh_token_get\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /visual_sightings/verify\n  method: get\n  operationId: verifyCarrierSighting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/agentic-access/genlogs-agentic-access.yml
summary_line: 28 operations · 17 acting
tags:
- Company
- Logistics
- Freight
- Trucking
- Supply Chain
- Carrier Intelligence
- Fleet
- Transportation
- Insurance
- Fraud Detection
- Webhooks
- Geospatial
---
