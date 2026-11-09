---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 19
api_specs:
- filename: leadboxer-com-credit-management-api-openapi.yml
  format: yaml
  label: leadboxer-com Credit Management API
  slug: leadboxer-com-credit-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-credit-management-api-openapi.yml
- filename: leadboxer-com-custom-tracking-domains-api-openapi.yml
  format: yaml
  label: leadboxer-com Custom Tracking Domains API
  slug: leadboxer-com-custom-tracking-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-custom-tracking-domains-api-openapi.yml
- filename: leadboxer-com-dataset-management-api-openapi.yml
  format: yaml
  label: leadboxer-com Dataset Management API
  slug: leadboxer-com-dataset-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-dataset-management-api-openapi.yml
- filename: leadboxer-com-leadoperation-api-openapi.yml
  format: yaml
  label: leadboxer-com Lead Operation API
  slug: leadboxer-com-leadoperation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-leadoperation-api-openapi.yml
- filename: leadboxer-com-leads-api-openapi.yml
  format: yaml
  label: leadboxer-com Leads API
  slug: leadboxer-com-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-leads-api-openapi.yml
- filename: leadboxer-com-log-api-openapi.yml
  format: yaml
  label: leadboxer-com Log API
  slug: leadboxer-com-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-log-api-openapi.yml
- filename: leadboxer-com-lookup-api-api-openapi.yml
  format: yaml
  label: leadboxer-com Lookup API
  slug: leadboxer-com-lookup-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-lookup-api-api-openapi.yml
- filename: leadboxer-com-segment-preference-api-openapi.yml
  format: yaml
  label: leadboxer-com Segment Preference API
  slug: leadboxer-com-segment-preference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-segment-preference-api-openapi.yml
- filename: leadboxer-com-segments-api-openapi.yml
  format: yaml
  label: leadboxer-com Segments API
  slug: leadboxer-com-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-segments-api-openapi.yml
- filename: leadboxer-com-track-api-api-openapi.yml
  format: yaml
  label: leadboxer-com Track API
  slug: leadboxer-com-track-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-track-api-api-openapi.yml
- filename: leadboxer-com-user-management-api-openapi.yml
  format: yaml
  label: leadboxer-com User Management API
  slug: leadboxer-com-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-user-management-api-openapi.yml
- filename: leadboxer-com-userdatasets-api-openapi.yml
  format: yaml
  label: leadboxer-com User Datasets API
  slug: leadboxer-com-userdatasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadboxer-com/openapi/leadboxer-com-userdatasets-api-openapi.yml
consequence_counts:
  read: 19
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Leadboxer Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'leadboxer-com exposes 42 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 23 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: leadboxer-com
provider_slug: leadboxer-com
slug: leadboxer-com-agentic-access
source_filename: leadboxer-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/leadboxer-com-api-openapi.yml, openapi/leadboxer-com-email-tracking-api-openapi.yml,\n  openapi/leadboxer-com-track-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 19\n    acting: 23\n  by_consequence:\n    read: 19\n    write: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/dataset-exclusion\n  method: get\n  operationId: getDatasetExclusions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dataset-exclusion\n  method: post\n  operationId: saveDatasetExclusion\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dataset-exclusion\n  method: delete\n  operationId: deleteDatasetExclusion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets\n  method: post\n  operationId: addDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}\n  method: delete\n  operationId:\
  \ removeDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/form-tracking\n  method: put\n  operationId: updateFormTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/name\n  method: put\n  operationId: updateDatasetName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/domain-lookup\n  method: get\n  operationId: lookupDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email-lookup\n  method: post\n  operationId: lookupEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email-lookup\n  method: get\n  operationId: lookupEmailByQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ip-lookup\n  method: get\n  operationId: lookupIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads\n  method: get\n  operationId: users\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads/events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads/export\n  method: get\n  operationId: usersCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads/sessions\n  method: get\n  operationId: getSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads/{leadId}\n  method: get\n  operationId: leadDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/management/assign-leads\n  method:\
  \ put\n  operationId: assignLeads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/management/credits\n  method: get\n  operationId: getAvailableCreditGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/management/ctd/add\n  method: post\n  operationId: addCustomTrackingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/management/ctd/update\n  method: put\n  operationId: updatedCustomTrackingDomain\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/management/ctd/validate\n  method: post\n  operationId: validateCustomTrackingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/management/ctd/{datasetId}\n  method: get\n  operationId: getCustomTrackingDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/management/ctd/{datasetId}\n  method: delete\n  operationId: deleteCustomTrackingDomain\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/management/lead-tags\n  method: put\n  operationId: updateLeadTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/segment/preference\n  method: get\n  operationId: getUsersBySegmentIdAndDatasetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segment/preference\n  method: put\n  operationId: saveDefaultSegment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/segment/preference\n  method: delete\n  operationId: deleteDefaultSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/segments\n  method: get\n  operationId: getSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments\n  method: post\n  operationId: createSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/segments/user\n  method: put\n  operationId: updateSegmentUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/segments/{segmentId}\n  method: put\n  operationId: updateSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/segments/{segmentId}\n  method: delete\n  operationId: deleteSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/user-datasets\n  method: get\n  operationId: getUserDatasets_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user-datasets\n  method: post\n  operationId: addUserDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/user-datasets\n  method: delete\n  operationId: removeUserDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users\n  method: post\n  operationId: addUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/datasets\n  method: get\n  operationId: getUserDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}\n  method: delete\n  operationId: removeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/users/{userId}/invite/resend\n  method: get\n  operationId: resendInvite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/name\n  method: put\n  operationId: updateName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /log\n  method: get\n  operationId: get_log\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: get_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/leadboxer-com/agentic-access/leadboxer-com-agentic-access.yml
summary_line: 42 operations · 23 acting
tags:
- B2B
- Lead Enrichment
- Marketing
- Data
---
