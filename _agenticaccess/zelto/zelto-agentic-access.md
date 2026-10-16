---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 26
api_specs:
- filename: zelto-action-checks-api-openapi.yml
  format: yaml
  label: Zelto Action checks API
  slug: zelto-action-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-action-checks-api-openapi.yml
- filename: zelto-agents-api-openapi.yml
  format: yaml
  label: Zelto Agents API
  slug: zelto-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-agents-api-openapi.yml
- filename: zelto-buckets-api-openapi.yml
  format: yaml
  label: Zelto Buckets API
  slug: zelto-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-buckets-api-openapi.yml
- filename: zelto-companies-api-openapi.yml
  format: yaml
  label: Zelto Companies API
  slug: zelto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-companies-api-openapi.yml
- filename: zelto-conversations-api-openapi.yml
  format: yaml
  label: Zelto Conversations API
  slug: zelto-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-conversations-api-openapi.yml
- filename: zelto-customer-metrics-api-openapi.yml
  format: yaml
  label: Zelto Customer Metrics API
  slug: zelto-customer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-customer-metrics-api-openapi.yml
- filename: zelto-experiments-api-openapi.yml
  format: yaml
  label: Zelto Experiments API
  slug: zelto-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-experiments-api-openapi.yml
- filename: zelto-findings-api-openapi.yml
  format: yaml
  label: Zelto Findings API
  slug: zelto-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-findings-api-openapi.yml
- filename: zelto-organizations-api-openapi.yml
  format: yaml
  label: Zelto Organizations API
  slug: zelto-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-organizations-api-openapi.yml
- filename: zelto-reports-api-openapi.yml
  format: yaml
  label: Zelto Reports API
  slug: zelto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-reports-api-openapi.yml
- filename: zelto-reviews-api-openapi.yml
  format: yaml
  label: Zelto Reviews API
  slug: zelto-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-reviews-api-openapi.yml
consequence_counts:
  physical: 1
  read: 26
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zelto Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/organizations
operation_count: 49
overview: 'Zelto exposes 49 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 22 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zelto
provider_slug: zelto
slug: zelto-agentic-access
source_filename: zelto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: generated\nsource: openapi/zelto-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 26\n    acting: 23\n  by_consequence:\n    read: 26\n    write: 22\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/reports/monitors/{reportId}\n  method: get\n  operationId: getMonitorReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}\n\
  \  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{id}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{id}/transcript\n  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{id}/customer-metrics\n  method: get\n  operationId: listCustomerMetrics\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{id}/customer-metrics\n  method: post\n  operationId: createCustomerMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/calls\n  method: post\n  operationId: uploadCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recording-uploads\n  method: post\n  operationId: createRecordingUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reviews\n  method: get\n  operationId: listReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}\n  method: get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/buckets\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/buckets\n  method: post\n  operationId: createBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/buckets/{id}\n  method: get\n  operationId: getBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/buckets/{id}/conversations\n  method: get\n  operationId: listBucketConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/buckets/{id}/conversations\n  method: post\n  operationId: addConversationToBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/buckets/{id}/conversations/{conversationId}\n  method: delete\n  operationId: removeConversationFromBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{id}\n  method: patch\n  operationId: updateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{id}/logo\n  method: put\n  operationId: uploadCompanyLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{id}/logo\n  method: delete\n  operationId: deleteCompanyLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/findings\n  method: get\n  operationId: listFindings\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/findings\n  method: post\n  operationId: createFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/findings/{id}\n  method: get\n  operationId: getFinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/findings/{id}\n  method: patch\n  operationId: updateFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/findings/{id}/conversations\n  method: get\n  operationId: listFindingConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/findings/{id}/conversations\n  method: post\n  operationId: addConversationToFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/findings/{id}/conversations/{conversationId}\n  method: delete\n  operationId: removeConversationFromFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /v1/findings/{id}/conversations/{conversationId}/comments\n  method: get\n  operationId: listFindingConversationComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/findings/{id}/conversations/{conversationId}/comments\n  method: post\n  operationId: createFindingConversationComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments/monitor-groups\n  method: get\n  operationId: listExperimentMonitorGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/experiments/preflight\n\
  \  method: post\n  operationId: preflightExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments\n  method: get\n  operationId: listExperiments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/experiments\n  method: post\n  operationId: createExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments/{id}\n  method: get\n  operationId: getExperiment\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/experiments/{id}\n  method: patch\n  operationId: updateExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments/{id}\n  method: delete\n  operationId: deleteExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments/{id}/conclude\n  method: post\n  operationId: concludeExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments/{id}/evaluations\n  method: get\n  operationId: listExperimentEvaluations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/experiments/{id}/evaluations\n  method: post\n  operationId: startExperimentEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experiments/{id}/evaluations/{runId}\n  method: get\n  operationId: getExperimentEvaluation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/experiments/{id}/conversations\n  method: get\n  operationId: listExperimentConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/action-checks\n  method: post\n  operationId: checkProposedAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/costs\n  method: get\n  operationId: getCostReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/transfers\n  method: get\n  operationId: getTransferReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}/versions\n  method: post\n  operationId: registerAgentVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/agentic-access/zelto-agentic-access.yml
summary_line: 49 operations · 23 acting
tags:
- Company
- VoiceAI
- QA
- Production
- Analytics
- Monitoring
---
