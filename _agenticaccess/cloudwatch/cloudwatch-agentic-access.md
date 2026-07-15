---
acting_count: 25
action_class_counts:
  acting: 25
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch API
  slug: amazon-cloudwatch-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/monitoring/2010-08-01/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Logs API
  slug: amazon-cloudwatch-logs-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/logs/2014-03-28/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Events API
  slug: amazon-cloudwatch-events-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/events/2015-10-07/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Application Insights API
  slug: amazon-cloudwatch-application-insights-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/application-insights/2018-11-25/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Synthetics API
  slug: amazon-cloudwatch-synthetics-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/synthetics/2017-10-11/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Internet Monitor API
  slug: amazon-cloudwatch-internet-monitor-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/internetmonitor/2021-06-03/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch RUM API
  slug: amazon-cloudwatch-rum-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/rum/2018-05-10/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon CloudWatch Observability Access Manager API
  slug: amazon-cloudwatch-observability-access-manager-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/oam/2022-06-10/openapi.yaml
consequence_counts:
  safety-critical: 1
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudwatch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#DisableAlarmActions
operation_count: 25
overview: 'AWS CloudWatch exposes 25 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 write and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWS CloudWatch
provider_slug: cloudwatch
slug: cloudwatch-agentic-access
source_filename: cloudwatch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudwatch-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 25\n  by_consequence:\n    write: 24\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: post\n  operationId: PutMetricData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetMetricData\n  method: post\n  operationId: GetMetricData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetMetricStatistics\n  method: post\n  operationId: GetMetricStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListMetrics\n  method: post\n  operationId: ListMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#PutMetricAlarm\n  method: post\n  operationId: PutMetricAlarm\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#PutCompositeAlarm\n  method: post\n  operationId: PutCompositeAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeAlarms\n  method: post\n  operationId: DescribeAlarms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeAlarmsForMetric\n \
  \ method: post\n  operationId: DescribeAlarmsForMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeAlarmHistory\n  method: post\n  operationId: DescribeAlarmHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DeleteAlarms\n  method: post\n  operationId: DeleteAlarms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /#SetAlarmState\n  method: post\n  operationId: SetAlarmState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#EnableAlarmActions\n  method: post\n  operationId: EnableAlarmActions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DisableAlarmActions\n  method: post\n  operationId: DisableAlarmActions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#PutDashboard\n  method: post\n  operationId: PutDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetDashboard\n  method: post\n  operationId: GetDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListDashboards\n  method: post\n  operationId: ListDashboards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DeleteDashboards\n  method: post\n  operationId: DeleteDashboards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#PutAnomalyDetector\n  method: post\n  operationId: PutAnomalyDetector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeAnomalyDetectors\n  method: post\n  operationId: DescribeAnomalyDetectors\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DeleteAnomalyDetector\n  method: post\n  operationId: DeleteAnomalyDetector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#PutMetricStream\n  method: post\n  operationId: PutMetricStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListMetricStreams\n\
  \  method: post\n  operationId: ListMetricStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /#ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/agentic-access/cloudwatch-agentic-access.yml
summary_line: 25 operations · 25 acting · 1 human-in-the-loop
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
---
