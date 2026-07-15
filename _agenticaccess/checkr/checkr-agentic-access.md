---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 35
api_specs:
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Candidates API
  slug: checkr-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Invitations API
  slug: checkr-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Reports API
  slug: checkr-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Screenings API
  slug: checkr-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Verifications API
  slug: checkr-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Packages API
  slug: checkr-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Documents API
  slug: checkr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Adverse Actions API
  slug: checkr-adverse-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Subscriptions API
  slug: checkr-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Continuous Checks API
  slug: checkr-continuous-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Nodes and Hierarchy API
  slug: checkr-nodes-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Geos API
  slug: checkr-geos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
- filename: checkr-openapi.yml
  format: yaml
  label: Checkr Webhooks API
  slug: checkr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/openapi/checkr-openapi.yml
consequence_counts:
  read: 35
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Checkr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 60
overview: 'Checkr exposes 60 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read and 25 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Checkr
provider_slug: checkr
slug: checkr-agentic-access
source_filename: checkr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/checkr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 60\n  by_action_class:\n    connected: 35\n    acting: 25\n  by_consequence:\n    read: 35\n    write: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /candidates\n  method: get\n  operationId: listCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates\n  method: post\n  operationId: createCandidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /candidates/{id}\n  method: get\n  operationId: getCandidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates/{id}\n  method: post\n  operationId: updateCandidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /candidates/{id}\n  method: delete\n  operationId: deleteCandidatePII\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /candidates/{id}/documents\n  method: get\n  operationId: listCandidateDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates/{id}/documents\n  method: post\n  operationId: uploadCandidateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /candidates/{id}/documents/{document_id}\n  method: get\n  operationId: getCandidateDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: get\n  operationId: listInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: post\n  operationId: createInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invitations/{id}\n  method: get\n  operationId: getInvitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations/{id}\n  method: delete\n  operationId: cancelInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports\n\
  \  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{id}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}\n  method: post\n  operationId: updateReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{id}/complete\n  method: post\n  operationId: completeReport\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{id}/eta\n  method: get\n  operationId: getReportEta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/ssn_trace/{id}\n  method: get\n  operationId: getSsnTrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/county_criminal_searches/{id}\n  method: get\n  operationId: getCountyCriminalSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/national_criminal_search/{id}\n\
  \  method: get\n  operationId: getNationalCriminalSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/federal_criminal_search/{id}\n  method: get\n  operationId: getFederalCriminalSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/sex_offender_search/{id}\n  method: get\n  operationId: getSexOffenderSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/motor_vehicle_report/{id}\n  method: get\n  operationId: getMotorVehicleReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/verifications\n\
  \  method: get\n  operationId: listVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/verifications/{id}\n  method: get\n  operationId: getVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{id}\n  method: get\n  operationId: getPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs\n  method: get\n  operationId: listPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{id}\n  method: get\n  operationId: getProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}/adverse_actions\n  method: get\n  operationId: listAdverseActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}/adverse_actions\n  method: post\n  operationId: createAdverseAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adverse_actions/{id}\n  method: get\n  operationId: getAdverseAction\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adverse_actions/{id}\n  method: delete\n  operationId: cancelAdverseAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /subscriptions/{id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n  method: post\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{id}\n  method: delete\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /continuous_checks\n  method: get\n\
  \  operationId: listContinuousChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /continuous_checks\n  method: post\n  operationId: createContinuousCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /continuous_checks/{id}\n  method: get\n  operationId: getContinuousCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /continuous_checks/{id}\n  method: delete\n  operationId: cancelContinuousCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hierarchy\n  method: post\n  operationId: createHierarchy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hierarchy/nodes\n  method: post\n  operationId: addHierarchyNodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hierarchy/status\n  method: get\n  operationId: getHierarchyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes\n  method: get\n  operationId: listNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes/{id}\n  method: get\n  operationId: getNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes/{id}\n  method: patch\n  operationId: updateNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nodes/{id}\n  method: delete\n  operationId: deleteNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geos\n  method: get\n  operationId: listGeos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geos\n  method: post\n  operationId: createGeo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geos/{id}\n  method: get\n  operationId: getGeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geos/{id}\n  method: post\n  operationId: updateGeo\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geos/{id}\n  method: delete\n  operationId: deleteGeo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkr/refs/heads/main/agentic-access/checkr-agentic-access.yml
summary_line: 60 operations · 25 acting
tags:
- Background Checks
- Employment Screening
- Compliance
- HR Tech
- Identity Verification
- Criminal Records
---
