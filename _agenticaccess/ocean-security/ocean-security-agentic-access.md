---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 17
api_specs:
- filename: ocean-security-openapi.yml
  format: yaml
  label: Ocean Security API
  slug: ocean-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-security/refs/heads/main/openapi/ocean-security-openapi.yml
consequence_counts:
  read: 17
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ocean Security Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Ocean Security exposes 20 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ocean Security
provider_slug: ocean-security
slug: ocean-security-agentic-access
source_filename: ocean-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/ocean-security-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 17\n    acting: 3\n  by_consequence:\n    read: 17\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/metrics/hours_saved\n  method: get\n  operationId: getHoursSavedMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/metrics/prevented_loss\n  method: get\n  operationId: getPreventedFinancialLoss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/metrics/protected_inboxes\n  method: get\n  operationId: getProtectedInboxesCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/metrics/threats_over_time\n  method: get\n  operationId: getThreatsOverTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/metrics/highlighted_threats\n  method: get\n  operationId: getTopHighlightedThreats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/metrics/top_targeted_entities\n  method: get\n  operationId: getTopTargetedEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/metrics/top_threat_types\n\
  \  method: get\n  operationId: getTopThreatTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/settings/allow_deny_entries\n  method: post\n  operationId: createAllowDenyEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/settings/allow_deny_entries\n  method: get\n  operationId: listAllowDenyEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/settings/allow_deny_entries/{id}\n  method: delete\n  operationId: deleteAllowDenyEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/settings/allow_deny_entries/{id}\n  method: patch\n  operationId: updateAllowDenyEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sonar/phishing-reports/aggs/verdicts\n  method: get\n  operationId: getAggregatedVerdicts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sonar/phishing-reports/aggs/mttr\n  method: get\n  operationId: getPhishingReportsMttr\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sonar/phishing-reports/{id}\n  method: get\n  operationId: getPhishingReportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sonar/phishing-reports/by_original_email_internet_message_id/{internet_message_id}\n  method: get\n  operationId: getPhishingReportsByOriginalEmailInternetMessageId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sonar/phishing-reports/by_report_internet_message_id/{internet_message_id}\n  method: get\n  operationId: getPhishingReportsByReportInternetMessageId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sonar/phishing-reports\n\
  \  method: get\n  operationId: listPhishingReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threats/{id}\n  method: get\n  operationId: getThreatById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threats/by_internet_message_id/{id}\n  method: get\n  operationId: getThreatsByInternetMessageId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threats\n  method: get\n  operationId: listRecentThreats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-security/refs/heads/main/agentic-access/ocean-security-agentic-access.yml
summary_line: 20 operations · 3 acting
tags:
- Company
- Security
- Email Security
- Cybersecurity
- Phishing
- Threat Detection
- Email
- Anti-Phishing
- Artificial Intelligence
- Threat Intelligence
---
