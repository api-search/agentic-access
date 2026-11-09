---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 8
api_specs:
- filename: getlulu-dev-c-api-openapi.yml
  format: yaml
  label: getlulu-dev C API
  slug: getlulu-dev-c-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-c-api-openapi.yml
- filename: getlulu-dev-campaigns-api-openapi.yml
  format: yaml
  label: getlulu-dev Campaigns API
  slug: getlulu-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-campaigns-api-openapi.yml
- filename: getlulu-dev-cron-api-openapi.yml
  format: yaml
  label: getlulu-dev Cron API
  slug: getlulu-dev-cron-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-cron-api-openapi.yml
- filename: getlulu-dev-health-api-openapi.yml
  format: yaml
  label: getlulu-dev Health API
  slug: getlulu-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-health-api-openapi.yml
- filename: getlulu-dev-i-api-openapi.yml
  format: yaml
  label: getlulu-dev I API
  slug: getlulu-dev-i-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-i-api-openapi.yml
- filename: getlulu-dev-install-md-api-openapi.yml
  format: yaml
  label: getlulu-dev Install.md API
  slug: getlulu-dev-install-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-install-md-api-openapi.yml
- filename: getlulu-dev-postback-api-openapi.yml
  format: yaml
  label: getlulu-dev Postback API
  slug: getlulu-dev-postback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-postback-api-openapi.yml
- filename: getlulu-dev-publishers-api-openapi.yml
  format: yaml
  label: getlulu-dev Publishers API
  slug: getlulu-dev-publishers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-publishers-api-openapi.yml
- filename: getlulu-dev-readme-sponsor-api-openapi.yml
  format: yaml
  label: getlulu-dev Readme Sponsor API
  slug: getlulu-dev-readme-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-readme-sponsor-api-openapi.yml
- filename: getlulu-dev-reports-api-openapi.yml
  format: yaml
  label: getlulu-dev Reports API
  slug: getlulu-dev-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-reports-api-openapi.yml
- filename: getlulu-dev-rewards-api-openapi.yml
  format: yaml
  label: getlulu-dev Rewards API
  slug: getlulu-dev-rewards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-rewards-api-openapi.yml
- filename: getlulu-dev-slot-api-openapi.yml
  format: yaml
  label: getlulu-dev Slot API
  slug: getlulu-dev-slot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-slot-api-openapi.yml
- filename: getlulu-dev-telemetry-api-openapi.yml
  format: yaml
  label: getlulu-dev Telemetry API
  slug: getlulu-dev-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlulu-dev/openapi/getlulu-dev-telemetry-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Getlulu Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cron/travelpayouts-poll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reports/payouts
operation_count: 22
overview: 'getlulu-dev exposes 22 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: getlulu-dev
provider_slug: getlulu-dev
slug: getlulu-dev-agentic-access
source_filename: getlulu-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/getlulu-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 14\n    connected: 8\n  by_consequence:\n    write: 12\n    read: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /postback/awin\n  method: post\n  operationId: awin_webhook_postback_awin_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: post\n  operationId: create_campaign_campaigns_post\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /i/{token}\n  method: get\n  operationId: impression_i__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/{token}\n  method: get\n  operationId: click_c__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postback\n  method: post\n  operationId: postback_postback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /cron/travelpayouts-poll\n  method: post\n  operationId: travelpayouts_poll_cron_travelpayouts_poll_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cron/adsterra-poll\n  method: post\n  operationId: adsterra_poll_cron_adsterra_poll_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cron/prospect-pitch-check\n  method: post\n  operationId: prospect_pitch_check_cron_prospect_pitch_check_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cron/poc-followup\n  method: post\n  operationId: poc_followup_cron_poc_followup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cron/outreach-followup\n  method: post\n  operationId: outreach_followup_cron_outreach_followup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /reports/prospects\n  method: get\n  operationId: prospects_report_reports_prospects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/prospects/by-publisher\n  method: get\n  operationId: prospects_by_publisher_report_reports_prospects_by_publisher_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers\n  method: post\n  operationId: create_publisher_publishers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publishers/verify\n  method: post\n  operationId: verify_publisher_publishers_verify_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /readme-sponsor/{slug}\n  method: get\n  operationId: readme_sponsor_readme_sponsor__slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/payouts\n  method: get\n  operationId: payouts_report_reports_payouts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/payouts\n  method: post\n  operationId: record_payout_reports_payouts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rewards/redeem\n  method: post\n  operationId: redeem_reward_rewards_redeem_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /slot\n  method: post\n  operationId: slot_slot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /telemetry/init\n  method: post\n  operationId: telemetry_init_telemetry_init_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /install.md\n  method: get\n  operationId: install_md_install_md_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/getlulu-dev/agentic-access/getlulu-dev-agentic-access.yml
summary_line: 22 operations · 14 acting
tags:
- Advertising
- Monetization
- Artificial Intelligence
- MCP
- Software-as-a-Service
---
