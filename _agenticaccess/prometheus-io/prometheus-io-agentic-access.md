---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 43
api_specs:
- filename: prometheus-io-admin-api-openapi.yml
  format: yaml
  label: Prometheus Admin API
  slug: prometheus-io-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-admin-api-openapi.yml
- filename: prometheus-io-alert-api-openapi.yml
  format: yaml
  label: Prometheus Alert API
  slug: prometheus-io-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-alert-api-openapi.yml
- filename: prometheus-io-alertgroup-api-openapi.yml
  format: yaml
  label: Prometheus Alertgroup API
  slug: prometheus-io-alertgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-alertgroup-api-openapi.yml
- filename: prometheus-io-alerts-api-openapi.yml
  format: yaml
  label: Prometheus Alerts API
  slug: prometheus-io-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-alerts-api-openapi.yml
- filename: prometheus-io-features-api-openapi.yml
  format: yaml
  label: Prometheus Features API
  slug: prometheus-io-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-features-api-openapi.yml
- filename: prometheus-io-general-api-openapi.yml
  format: yaml
  label: Prometheus General API
  slug: prometheus-io-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-general-api-openapi.yml
- filename: prometheus-io-labels-api-openapi.yml
  format: yaml
  label: Prometheus Labels API
  slug: prometheus-io-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-labels-api-openapi.yml
- filename: prometheus-io-metadata-api-openapi.yml
  format: yaml
  label: Prometheus Metadata API
  slug: prometheus-io-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-metadata-api-openapi.yml
- filename: prometheus-io-notifications-api-openapi.yml
  format: yaml
  label: Prometheus Notifications API
  slug: prometheus-io-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-notifications-api-openapi.yml
- filename: prometheus-io-otlp-api-openapi.yml
  format: yaml
  label: Prometheus Otlp API
  slug: prometheus-io-otlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-otlp-api-openapi.yml
- filename: prometheus-io-query-api-openapi.yml
  format: yaml
  label: Prometheus Query API
  slug: prometheus-io-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-query-api-openapi.yml
- filename: prometheus-io-receiver-api-openapi.yml
  format: yaml
  label: Prometheus Receiver API
  slug: prometheus-io-receiver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-receiver-api-openapi.yml
- filename: prometheus-io-remote-api-openapi.yml
  format: yaml
  label: Prometheus Remote API
  slug: prometheus-io-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-remote-api-openapi.yml
- filename: prometheus-io-rules-api-openapi.yml
  format: yaml
  label: Prometheus Rules API
  slug: prometheus-io-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-rules-api-openapi.yml
- filename: prometheus-io-series-api-openapi.yml
  format: yaml
  label: Prometheus Series API
  slug: prometheus-io-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-series-api-openapi.yml
- filename: prometheus-io-silence-api-openapi.yml
  format: yaml
  label: Prometheus Silence API
  slug: prometheus-io-silence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-silence-api-openapi.yml
- filename: prometheus-io-status-api-openapi.yml
  format: yaml
  label: Prometheus Status API
  slug: prometheus-io-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-status-api-openapi.yml
- filename: prometheus-io-targets-api-openapi.yml
  format: yaml
  label: Prometheus Targets API
  slug: prometheus-io-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-targets-api-openapi.yml
consequence_counts:
  read: 43
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prometheus Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 57
overview: 'Prometheus exposes 57 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 43 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prometheus
provider_slug: prometheus-io
slug: prometheus-io-agentic-access
source_filename: prometheus-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/prometheus-io-admin-api-openapi.yml, openapi/prometheus-io-alert-api-openapi.yml,\n  openapi/prometheus-io-alertgroup-api-openapi.yml, openapi/prometheus-io-alerts-api-openapi.yml,\n  openapi/prometheus-io-features-api-openapi.yml, openapi/prometheus-io-general-api-openapi.yml,\n  openapi/prometheus-io-labels-api-openapi.yml, openapi/prometheus-io-metadata-api-openapi.yml,\n  openapi/prometheus-io-notifications-api-openapi.yml, openapi/prometheus-io-otlp-api-openapi.yml,\n  openapi/prometheus-io-query-api-openapi.yml, openapi/prometheus-io-receiver-api-openapi.yml,\n  openapi/prometheus-io-remote-api-openapi.yml, openapi/prometheus-io-rules-api-openapi.yml,\n  openapi/prometheus-io-series-api-openapi.yml, openapi/prometheus-io-silence-api-openapi.yml,\n  openapi/prometheus-io-status-api-openapi.yml, openapi/prometheus-io-targets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified\
  \ heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    acting: 14\n    connected: 43\n  by_consequence:\n    write: 14\n    read: 43\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/tsdb/delete_series\n  method: put\n  operationId: deleteSeriesPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tsdb/delete_series\n  method: post\n  operationId: deleteSeriesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tsdb/clean_tombstones\n  method: put\n  operationId: cleanTombstonesPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tsdb/clean_tombstones\n  method: post\n  operationId: cleanTombstonesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tsdb/snapshot\n  method: put\n  operationId: snapshotPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tsdb/snapshot\n  method: post\n  operationId: snapshotPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts\n  method: get\n  operationId: getAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: post\n  operationId: postAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /alerts/groups\n  method: get\n  operationId: getAlertGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n  operationId: alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alertmanagers\n  method: get\n  operationId: alertmanagers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /features\n  method: get\n  operationId: get-features\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: get\n  operationId: labels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: post\n  operationId: labels-post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /label/{name}/values\n  method: get\n  operationId: label-values\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/label_names\n  method: get\n  operationId: search-label-names\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/label_names\n  method: post\n  operationId:\
  \ search-label-names-post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/label_values\n  method: get\n  operationId: search-label-values\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/label_values\n  method: post\n  operationId: search-label-values-post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/metric_names\n  method: get\n  operationId: search-metric-names\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/metric_names\n  method: post\n  operationId: search-metric-names-post\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: get-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: get\n  operationId: get-notifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /otlp/v1/metrics\n  method: post\n  operationId: otlpWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query\n  method: get\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: post\n  operationId: query-post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query_range\n  method: get\n  operationId: query-range\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query_range\n  method: post\n  operationId: query-range-post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query_exemplars\n  method: get\n  operationId: query-exemplars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query_exemplars\n  method: post\n  operationId: query-exemplars-post\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /format_query\n  method: get\n  operationId: format-query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /format_query\n  method: post\n  operationId: format-query-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parse_query\n  method: get\n  operationId: parse-query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parse_query\n  method: post\n  operationId: parse-query-post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receivers\n  method: get\n  operationId: getReceivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read\n  method: post\n  operationId: remoteRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write\n  method: post\n  operationId: remoteWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules\n  method: get\n  operationId: rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series\n  method: get\n  operationId: series\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series\n  method: post\n  operationId: series-post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /silences\n  method: get\n  operationId: getSilences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /silences\n  method: post\n  operationId: postSilences\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /silence/{silenceID}\n  method: get\n  operationId: getSilence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /silence/{silenceID}\n  method: delete\n  operationId: deleteSilence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/config\n  method: get\n  operationId: get-status-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/runtimeinfo\n  method: get\n  operationId: get-status-runtimeinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/buildinfo\n  method: get\n  operationId: get-status-buildinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/flags\n  method: get\n  operationId: get-status-flags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/tsdb\n  method: get\n  operationId: status-tsdb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/tsdb/blocks\n  method: get\n  operationId: status-tsdb-blocks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/walreplay\n  method: get\n  operationId: get-status-walreplay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/self_metrics\n  method: get\n  operationId: get-status-self-metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scrape_pools\n  method: get\n  operationId: get-scrape-pools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /targets\n  method: get\n  operationId: get-targets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /targets/metadata\n  method: get\n  operationId: get-targets-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /targets/relabel_steps\n  method: get\n  operationId: get-targets-relabel-steps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/agentic-access/prometheus-io-agentic-access.yml
summary_line: 57 operations · 14 acting
tags:
- Prometheus
- Monitoring
- Metrics
- Observability
- Time Series
- Alerting
- Cloud-Native
- CNCF
- Open Source
- PromQL
- Telemetry
---
