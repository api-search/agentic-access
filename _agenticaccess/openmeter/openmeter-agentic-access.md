---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 22
api_specs:
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Events Ingestion API
  slug: openmeter-events-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Meters API
  slug: openmeter-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Usage Query API
  slug: openmeter-usage-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Subjects API
  slug: openmeter-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Entitlements API
  slug: openmeter-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Features API
  slug: openmeter-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Grants API
  slug: openmeter-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Notifications API
  slug: openmeter-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Billing and Plans API
  slug: openmeter-billing-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
consequence_counts:
  read: 22
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openmeter Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'OpenMeter exposes 36 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenMeter
provider_slug: openmeter
slug: openmeter-agentic-access
source_filename: openmeter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openmeter-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 22\n    acting: 14\n  by_consequence:\n    read: 22\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events\n  method: post\n  operationId: ingestEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/meters\n  method: get\n  operationId: listMeters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meters\n  method: post\n  operationId: createMeter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/meters/{meterIdOrSlug}\n  method: get\n  operationId: getMeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meters/{meterIdOrSlug}\n  method: delete\n  operationId: deleteMeter\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/meters/{meterIdOrSlug}/query\n  method: get\n  operationId: queryMeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meters/{meterIdOrSlug}/subjects\n  method: get\n  operationId: listMeterSubjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subjects\n  method: get\n  operationId: listSubjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subjects\n  method: post\n  operationId: upsertSubject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subjects/{subjectIdOrKey}\n  method: get\n  operationId: getSubject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subjects/{subjectIdOrKey}\n  method: delete\n  operationId: deleteSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/features\n  method: get\n  operationId: listFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/features\n  method: post\n  operationId: createFeature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/features/{featureId}\n\
  \  method: get\n  operationId: getFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/features/{featureId}\n  method: delete\n  operationId: deleteFeature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entitlements\n  method: get\n  operationId: listEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entitlements/{entitlementId}\n  method: get\n  operationId: getEntitlementById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/subjects/{subjectIdOrKey}/entitlements\n  method: get\n  operationId: listSubjectEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subjects/{subjectIdOrKey}/entitlements\n  method: post\n  operationId: createEntitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subjects/{subjectIdOrKey}/entitlements/{entitlementIdOrFeatureKey}/value\n  method: get\n  operationId: getEntitlementValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subjects/{subjectIdOrKey}/entitlements/{entitlementIdOrFeatureKey}/grants\n\
  \  method: get\n  operationId: listEntitlementGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subjects/{subjectIdOrKey}/entitlements/{entitlementIdOrFeatureKey}/grants\n  method: post\n  operationId: createGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/grants\n  method: get\n  operationId: listGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/grants/{grantId}\n  method: delete\n  operationId: voidGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/notification/channels\n  method: get\n  operationId: listNotificationChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/notification/channels\n  method: post\n  operationId: createNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/notification/rules\n  method: get\n  operationId: listNotificationRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/notification/rules\n  method: post\n  operationId: createNotificationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/notification/events\n  method: get\n  operationId: listNotificationEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/profiles\n  method: get\n  operationId: listBillingProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/agentic-access/openmeter-agentic-access.yml
summary_line: 36 operations · 14 acting
tags:
- Usage Metering
- Billing
- Entitlements
- CloudEvents
- Open Source
- AI
---
