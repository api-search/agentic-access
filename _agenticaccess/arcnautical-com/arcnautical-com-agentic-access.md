---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 37
api_specs:
- filename: arcnautical-com-account-api-openapi.yml
  format: yaml
  label: ArcNautical Account API
  slug: arcnautical-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-account-api-openapi.yml
- filename: arcnautical-com-cargo-screening-api-openapi.yml
  format: yaml
  label: ArcNautical Cargo screening API
  slug: arcnautical-com-cargo-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-cargo-screening-api-openapi.yml
- filename: arcnautical-com-corridor-monitors-api-openapi.yml
  format: yaml
  label: ArcNautical Corridor monitors API
  slug: arcnautical-com-corridor-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-corridor-monitors-api-openapi.yml
- filename: arcnautical-com-crew-placement-api-openapi.yml
  format: yaml
  label: ArcNautical Crew placement API
  slug: arcnautical-com-crew-placement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-crew-placement-api-openapi.yml
- filename: arcnautical-com-exports-api-openapi.yml
  format: yaml
  label: ArcNautical Exports API
  slug: arcnautical-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-exports-api-openapi.yml
- filename: arcnautical-com-fleets-api-openapi.yml
  format: yaml
  label: ArcNautical Fleets API
  slug: arcnautical-com-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-fleets-api-openapi.yml
- filename: arcnautical-com-port-lookup-api-openapi.yml
  format: yaml
  label: ArcNautical Port lookup API
  slug: arcnautical-com-port-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-port-lookup-api-openapi.yml
- filename: arcnautical-com-public-vessel-check-api-openapi.yml
  format: yaml
  label: ArcNautical Public vessel check API
  slug: arcnautical-com-public-vessel-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-public-vessel-check-api-openapi.yml
- filename: arcnautical-com-vessel-monitors-api-openapi.yml
  format: yaml
  label: ArcNautical Vessel monitors API
  slug: arcnautical-com-vessel-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-vessel-monitors-api-openapi.yml
- filename: arcnautical-com-vessel-screening-api-openapi.yml
  format: yaml
  label: ArcNautical Vessel screening API
  slug: arcnautical-com-vessel-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-vessel-screening-api-openapi.yml
- filename: arcnautical-com-voyage-assessments-api-openapi.yml
  format: yaml
  label: ArcNautical Voyage assessments API
  slug: arcnautical-com-voyage-assessments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-voyage-assessments-api-openapi.yml
- filename: arcnautical-com-webhooks-api-openapi.yml
  format: yaml
  label: ArcNautical Webhooks API
  slug: arcnautical-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 37
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arcnautical Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/crew-checks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/crew-ships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/crew-ships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhook-endpoints/{id}/test
operation_count: 64
overview: 'ArcNautical exposes 64 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 23 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ArcNautical
provider_slug: arcnautical-com
slug: arcnautical-com-agentic-access
source_filename: arcnautical-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arcnautical-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    connected: 37\n    acting: 27\n  by_consequence:\n    read: 37\n    write: 23\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/voyage-assessments\n  method: get\n  operationId: listVoyageAssessments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:score\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/voyage-assessments\n  method: post\n  operationId: createVoyageAssessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - voyage:score\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/voyage-assessments/{id}\n  method: get\n  operationId: getVoyageAssessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:score\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/voyage-assessment-batches\n  method: post\n  operationId: createVoyageAssessmentBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - voyage:score\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/voyage-assessment-batches/{id}\n  method: get\n  operationId: getVoyageAssessmentBatch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:score\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/voyage-assessment-batches/{id}/items\n  method: get\n  operationId: listVoyageAssessmentBatchItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:score\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/screenings\n  method: get\n  operationId: listScreenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/screenings\n  method: post\n  operationId: createScreening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/screenings/{id}\n  method: get\n  operationId: getScreening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fleets\n  method: post\n  operationId: createFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fleets\n  method: get\n  operationId: listFleets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/fleets/{id}\n  method: get\n  operationId: getFleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fleets/{id}\n  method: patch\n  operationId: updateFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fleets/{id}\n  method: delete\n  operationId: deleteFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/fleets/{id}/exposure\n  method: get\n  operationId: getFleetExposure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fleets/{id}/changes\n  method: get\n  operationId: getFleetChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fleets/{id}/refresh\n  method: post\n  operationId: refreshFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cargo-screenings\n  method: post\n  operationId: createCargoScreening\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cargo:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cargo-screenings\n  method: get\n  operationId: listCargoScreenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cargo:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cargo-screenings/{id}\n  method: get\n  operationId: getCargoScreening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cargo:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/screening-batches\n  method: post\n  operationId: createScreeningBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    scope:\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/screening-batches/{id}\n  method: get\n  operationId: getScreeningBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/screening-batches/{id}/items\n  method: get\n  operationId: listScreeningBatchItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vessel-monitors\n  method: post\n  operationId: createVesselMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:monitor\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/vessel-monitors\n  method: get\n  operationId: listVesselMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vessel-monitors/batch\n  method: post\n  operationId: createVesselMonitorsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/vessel-monitors/events\n  method: get\n  operationId: listVesselMonitorEvents\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - vessel:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vessel-monitors/{id}\n  method: get\n  operationId: getVesselMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vessel-monitors/{id}\n  method: patch\n  operationId: updateVesselMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/vessel-monitors/{id}\n  method: delete\n  operationId: deleteVesselMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n  \
  \  - vessel:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/vessel-monitors/{id}/history\n  method: get\n  operationId: getVesselMonitorHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - vessel:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vessel-monitors/{id}/simulate\n  method: post\n  operationId: simulateVesselMonitorEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - vessel:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/corridor-monitors\n  method: post\n  operationId: createCorridorMonitor\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - voyage:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/corridor-monitors\n  method: get\n  operationId: listCorridorMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/corridor-monitors/{id}\n  method: get\n  operationId: getCorridorMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/corridor-monitors/{id}\n  method: patch\n  operationId: updateCorridorMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - voyage:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/corridor-monitors/{id}\n  method: delete\n  operationId: deleteCorridorMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - voyage:monitor\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/corridor-monitors/{id}/history\n  method: get\n  operationId: getCorridorMonitorHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - voyage:monitor\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints\n  method: post\n  operationId: createWebhookEndpoint\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:manage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/{id}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:manage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/{id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - webhooks:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints/{id}/test\n  method: post\n  operationId: testWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - webhooks:manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:manage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-deliveries/{id}\n  method: get\n  operationId: getWebhookDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:manage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-deliveries/{id}/redeliver\n  method: post\n  operationId: redeliverWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cargo:screen\n    - logs:read\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports\n  method: get\n  operationId: listExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cargo:screen\n    - logs:read\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exports/{id}\n  method: get\n  operationId: getExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cargo:screen\n    - logs:read\n    -\
  \ vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exports/{id}\n  method: delete\n  operationId: deleteExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cargo:screen\n    - logs:read\n    - vessel:screen\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports/{id}/download\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cargo:screen\n    - logs:read\n    - vessel:screen\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crew-checks\n  method: post\n  operationId: createCrewCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - crew:check\n   \
  \ audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crew-checks\n  method: get\n  operationId: listCrewChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - crew:check\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crew-checks/{id}\n  method: get\n  operationId: getCrewCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - crew:check\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crew-checks/{id}/pdf\n  method: get\n  operationId: downloadCrewCheckPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - crew:check\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/crew-ships\n  method: post\n  operationId: createCrewShip\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - crew:check\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crew-ships\n  method: get\n  operationId: listCrewShips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - crew:check\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crew-ships/{id}\n  method: get\n  operationId: getCrewShip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - crew:check\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crew-ships/{id}\n  method: delete\n  operationId:\
  \ deleteCrewShip\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - crew:check\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/access-log\n  method: get\n  operationId: getAccessLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - logs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - usage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vessels/{imo}/check\n  method: get\n  operationId: checkVesselPublic\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ports\n  method: get\n  operationId: searchPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/arcnautical-com/agentic-access/arcnautical-com-agentic-access.yml
summary_line: 64 operations · 27 acting
tags:
- Company
- Maritime
- Compliance
- Data
- Screening
---
