---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 18
api_specs:
- filename: leapfrog-power-create-meters-api-openapi.yml
  format: yaml
  label: Leap create meters API
  slug: leapfrog-power-create-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-create-meters-api-openapi.yml
- filename: leapfrog-power-group-dispatches-api-openapi.yml
  format: yaml
  label: Leap Group Dispatches API
  slug: leapfrog-power-group-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-group-dispatches-api-openapi.yml
- filename: leapfrog-power-interval-data-upload-api-openapi.yml
  format: yaml
  label: Leap Interval Data Upload API
  slug: leapfrog-power-interval-data-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-interval-data-upload-api-openapi.yml
- filename: leapfrog-power-meter-details-api-openapi.yml
  format: yaml
  label: Leap Meter Details API
  slug: leapfrog-power-meter-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-details-api-openapi.yml
- filename: leapfrog-power-meter-dispatches-api-openapi.yml
  format: yaml
  label: Leap Meter Dispatches API
  slug: leapfrog-power-meter-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-dispatches-api-openapi.yml
- filename: leapfrog-power-meter-enrollment-api-openapi.yml
  format: yaml
  label: Leap meter enrollment API
  slug: leapfrog-power-meter-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-meter-enrollment-api-openapi.yml
- filename: leapfrog-power-nominations-api-openapi.yml
  format: yaml
  label: Leap Nominations API
  slug: leapfrog-power-nominations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-nominations-api-openapi.yml
- filename: leapfrog-power-performance-api-openapi.yml
  format: yaml
  label: Leap Performance API
  slug: leapfrog-power-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-performance-api-openapi.yml
- filename: leapfrog-power-provisional-assets-api-openapi.yml
  format: yaml
  label: Leap provisional assets API
  slug: leapfrog-power-provisional-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-provisional-assets-api-openapi.yml
- filename: leapfrog-power-revenue-api-openapi.yml
  format: yaml
  label: Leap Revenue API
  slug: leapfrog-power-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-revenue-api-openapi.yml
- filename: leapfrog-power-webhooks-api-openapi.yml
  format: yaml
  label: Leap Webhooks API
  slug: leapfrog-power-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/openapi/leapfrog-power-webhooks-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 9
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Leapfrog Power Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/group/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /dispatch/group/webhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dispatch/group/webhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/group/webhook/integration_test
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/meter/communication_test
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/meter/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /dispatch/meter/webhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dispatch/meter/webhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dispatch/meter/webhook/integration_test
operation_count: 48
overview: 'Leap exposes 48 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 21 write, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Leap
provider_slug: leapfrog-power
slug: leapfrog-power-agentic-access
source_filename: leapfrog-power-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/leapfrog-power-create-meters-openapi.yml, openapi/leapfrog-power-dispatch-openapi.yml,\n  openapi/leapfrog-power-interval-data-upload-openapi.json, openapi/leapfrog-power-meter-details-openapi.yml,\n  openapi/leapfrog-power-meter-enrollment-openapi.yml, openapi/leapfrog-power-nominations-openapi.yml,\n  openapi/leapfrog-power-revenue-analytics-openapi.yml, openapi/leapfrog-power-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 18\n    acting: 30\n  by_consequence:\n    read: 18\n    write: 21\n    safety-critical: 9\n  human_in_the_loop_required: 9\noperations:\n- path: /v1.1/jobs/meters\n  method: get\n  operationId: listMeterBatchJobs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/jobs/meters\n  method: post\n  operationId: createMeterBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/jobs/meter-job-filters\n  method: get\n  operationId: listMeterBatchJobsFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/jobs/meters/{job_id}\n  method: get\n  operationId: getMeterBatchJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/meters\n  method:\
  \ post\n  operationId: createSingleMeter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/provisional-assets\n  method: get\n  operationId: listProvisionalAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/provisional-assets-filters\n  method: get\n  operationId: listProvisionalAssetsFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dispatch/meter/search\n  method: post\n  operationId: searchMeterDispatches\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/group/search\n  method: post\n  operationId: searchGroupDispatches\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/meter/communication_test\n  method: post\n  operationId: triggerCommunicationTestMeterDispatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /dispatch/meter/webhook\n  method: delete\n  operationId: deleteMeterDispatchWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/meter/webhook\n  method: get\n  operationId: getMeterDispatchWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dispatch/meter/webhook\n  method: put\n  operationId: createOrUpdateMeterDispatchWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/meter/webhook/integration_test\n  method: post\n  operationId: triggerTestMeterDispatchNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/group/webhook\n  method: delete\n  operationId: deleteGroupDispatchWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/group/webhook\n  method: get\n  operationId: getGroupDispatchWebhook\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dispatch/group/webhook\n  method: put\n  operationId: createOrUpdateGroupDispatchWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dispatch/group/webhook/integration_test\n  method: post\n  operationId: triggerTestGroupDispatchNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /v1.1/jobs/interval-data-uploads\n  method: get\n  operationId: listIntervalDataUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/jobs/interval-data-uploads/{job_id}\n  method: get\n  operationId: listIntervalDataUploadErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/jobs/interval-data-uploads/presigned-url/{job_id}\n  method: get\n  operationId: intervalDataPresignedUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/jobs/interval-data-uploads/file-preview/{job_id}\n  method: get\n  operationId: intervalDataFilePreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1.1/missing-interval-data/search\n  method: post\n  operationId: searchMissingIntervalData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/interval-data\n  method: post\n  operationId: uploadIntervalData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/meters/{meter_id}\n  method: get\n  operationId: getMeterDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/meters/search\n\
  \  method: post\n  operationId: searchMeterDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/meters/{meter_id}/enrollments\n  method: get\n  operationId: getMeterEnrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/meters/enrollments/search\n  method: post\n  operationId: searchMeterEnrollments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/meters/{meter_id}/nominations/suggestions\n  method:\
  \ get\n  operationId: getMeterNominationSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/meters/{meter_id}/nominations/suggestions\n  method: post\n  operationId: postMeterNominationSuggestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/meters/{meter_id}/nominations/suggestions/{nomination_suggestion_id}\n  method: delete\n  operationId: deleteMeterNominationSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /v2/meters/nominations/suggestions\n  method: post\n  operationId: postNominationSuggestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/meters/nominations/suggestions/search\n  method: post\n  operationId: searchNominationSuggestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/meters/nominations/search\n  method: post\n  operationId: searchNominations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/revenue/periodic/aggregation/customer/search\n  method: post\n  operationId: postCustomerSearchPeriodicAggregationSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/revenue/periodic/aggregation/load-type/search\n  method: post\n  operationId: postLoadTypeSearchPeriodicAggregationSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/revenue/periodic/aggregation/market-group/search\n\
  \  method: post\n  operationId: postMarketGroupSearchPeriodicAggregationSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/revenue/periodic/aggregation/meter/search\n  method: post\n  operationId: postMeterSearchPeriodicAggregationSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/revenue/periodic/aggregation/utility/search\n  method: post\n  operationId: postUtilitySearchPeriodicAggregationSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/revenue/periodic/reports\n  method: get\n  operationId: getPeriodicReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/revenue/periodic/versions\n  method: get\n  operationId: getPeriodicReportVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/revenue/yearly/{year}\n  method: get\n  operationId: getYearlyOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/performance/diagnosis/monthly/unresponsive/meters\n  method: post\n  operationId: postMonthlyUnresponsiveMetersPerformance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/webhooks/{webhook_id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/webhooks/{webhook_id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapfrog-power/refs/heads/main/agentic-access/leapfrog-power-agentic-access.yml
summary_line: 48 operations · 30 acting · 9 human-in-the-loop
tags:
- Energy
- United States
- Electricity
- Grid
- Demand Response
- DER
- Virtual Power Plant
- Energy Markets
- Storage Flexibility
- EV Charging
- Smart Metering
---
