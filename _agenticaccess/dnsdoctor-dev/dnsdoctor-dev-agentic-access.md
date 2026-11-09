---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: dnsdoctor-dev-domains-api-openapi.yml
  format: yaml
  label: DNS Doctor Domains API
  slug: dnsdoctor-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-domains-api-openapi.yml
- filename: dnsdoctor-dev-monitoring-api-openapi.yml
  format: yaml
  label: DNS Doctor Monitoring API
  slug: dnsdoctor-dev-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-monitoring-api-openapi.yml
- filename: dnsdoctor-dev-scan-api-openapi.yml
  format: yaml
  label: DNS Doctor Scan API
  slug: dnsdoctor-dev-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-scan-api-openapi.yml
- filename: dnsdoctor-dev-tools-api-openapi.yml
  format: yaml
  label: DNS Doctor Tools API
  slug: dnsdoctor-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-tools-api-openapi.yml
- filename: dnsdoctor-dev-watch-api-openapi.yml
  format: yaml
  label: DNS Doctor Watch API
  slug: dnsdoctor-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-watch-api-openapi.yml
consequence_counts:
  read: 9
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dnsdoctor Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'DNS Doctor exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DNS Doctor
provider_slug: dnsdoctor-dev
slug: dnsdoctor-dev-agentic-access
source_filename: dnsdoctor-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dnsdoctor-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 9\n    acting: 14\n  by_consequence:\n    read: 9\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /report/{domain}\n  method: get\n  operationId: report_report__domain__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scan\n  method: post\n  operationId: scan_scan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dmarc-upgrade\n  method: post\n  operationId: dmarc_upgrade_dmarc_upgrade_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signup-url\n  method: post\n  operationId: signup_url_signup_url_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains\n  method: get\n  operationId: domains_domains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /domains\n  method: post\n  operationId: add_domain_route_domains_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts\n  method: get\n  operationId: alerts_alerts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readiness\n  method: get\n  operationId: readiness_readiness_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/verify\n  method: post\n  operationId: verify_domain_route_domains_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/records\n  method: get\n  operationId: domain_records_route_domains_records_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/mine\n  method: get\n  operationId: my_domains_route_domains_mine_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change-watch\n  method: post\n  operationId: change_watch_route_change_watch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /lookalikes\n  method: get\n  operationId: lookalikes_lookalikes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-tests\n  method: get\n  operationId: email_tests_email_tests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk-scan\n  method: post\n  operationId: bulk_scan_bulk_scan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk-registration\n  method: post\n  operationId: bulk_registration_bulk_registration_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk-propagation\n  method: post\n  operationId: bulk_propagation_bulk_propagation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk-dmarc-reports\n  method: post\n  operationId: bulk_dmarc_reports_bulk_dmarc_reports_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/propagation\n  method:\
  \ post\n  operationId: create_propagation_watch_watch_propagation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/ping\n  method: post\n  operationId: create_ping_watch_watch_ping_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/record\n  method: post\n  operationId: create_record_watch_watch_record_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/lookalikes\n  method: post\n  operationId: create_lookalikes_watch_watch_lookalikes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/{watch_id}\n  method: get\n  operationId: poll_watch_watch__watch_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dnsdoctor-dev/agentic-access/dnsdoctor-dev-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- DNS
- DNS Tools
- Email Authentication
- Web Application
---
