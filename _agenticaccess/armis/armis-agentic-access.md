---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 17
api_specs:
- filename: armis-alerts-api-openapi.yml
  format: yaml
  label: Armis Alerts API
  slug: armis-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-alerts-api-openapi.yml
- filename: armis-arp-api-openapi.yml
  format: yaml
  label: Armis ARP API
  slug: armis-arp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-arp-api-openapi.yml
- filename: armis-assets-api-openapi.yml
  format: yaml
  label: Armis Assets API
  slug: armis-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-assets-api-openapi.yml
- filename: armis-authentication-api-openapi.yml
  format: yaml
  label: Armis Authentication API
  slug: armis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-authentication-api-openapi.yml
- filename: armis-boundaries-api-openapi.yml
  format: yaml
  label: Armis Boundaries API
  slug: armis-boundaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-boundaries-api-openapi.yml
- filename: armis-collectors-api-openapi.yml
  format: yaml
  label: Armis Collectors API
  slug: armis-collectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-collectors-api-openapi.yml
- filename: armis-data-export-api-openapi.yml
  format: yaml
  label: Armis Data Export API
  slug: armis-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-data-export-api-openapi.yml
- filename: armis-device-custom-properties-api-openapi.yml
  format: yaml
  label: Armis Device Custom Properties API
  slug: armis-device-custom-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-device-custom-properties-api-openapi.yml
- filename: armis-integrations-api-openapi.yml
  format: yaml
  label: Armis Integrations API
  slug: armis-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-integrations-api-openapi.yml
- filename: armis-policies-api-openapi.yml
  format: yaml
  label: Armis Policies API
  slug: armis-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-policies-api-openapi.yml
- filename: armis-sites-api-openapi.yml
  format: yaml
  label: Armis Sites API
  slug: armis-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/openapi/armis-sites-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Armis Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /data-export/{entity}
operation_count: 34
overview: 'Armis exposes 34 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Armis
provider_slug: armis
slug: armis-agentic-access
source_filename: armis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/armis-api-v3-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 17\n    acting: 17\n  by_consequence:\n    read: 17\n    write: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /alerts/{alert_id}\n  method: get\n  operationId: get_alerts__alert_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arps\n  method: post\n  operationId: post_arps_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/_bulk\n  method: post\n  operationId: post_assets__bulk_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/_search\n  method: post\n  operationId: search_assets__search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/_search/fields\n  method: get\n  operationId: fields_assets__search_fields_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collectors\n  method: get\n  operationId:\
  \ get_collectors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collectors/_image\n  method: get\n  operationId: get_collectors__image_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collectors/{collector_number}\n  method: get\n  operationId: get_collectors__collector_number__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-export/{entity}\n  method: get\n  operationId: get_data_export__entity__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-export/{entity}\n  method: patch\n  operationId: toggle_data_export__entity__patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /data-export/{entity}/_enable\n  method: post\n  operationId: enable_data_export__entity___enable_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: post_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /policies\n  method: get\n  operationId: get_policies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/boundaries\n  method: post\n  operationId: post_settings_boundaries_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/boundaries\n  method: get\n  operationId: get_settings_boundaries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/boundaries/{boundary_id}\n  method: delete\n  operationId: delete_settings_boundaries__boundary_id__delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/boundaries/{boundary_id}\n  method: get\n  operationId: get_settings_boundaries__boundary_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/boundaries/{boundary_id}\n  method: patch\n  operationId: patch_settings_boundaries__boundary_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/device-custom-properties\n  method: post\n  operationId: post_settings_device_custom_properties_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/device-custom-properties\n  method: get\n  operationId: get_settings_device_custom_properties_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/device-custom-properties/{config_id}\n  method: delete\n  operationId: delete_settings_device_custom_properties__config_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/device-custom-properties/{config_id}\n\
  \  method: get\n  operationId: get_settings_device_custom_properties__config_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/device-custom-properties/{config_id}\n  method: patch\n  operationId: patch_settings_device_custom_properties__config_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/integrations\n  method: get\n  operationId: get_settings_integrations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/integrations\n  method: post\n  operationId: post_settings_integrations_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/integrations/_search\n  method: post\n  operationId: search_settings_integrations__search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/integrations/{integration_id}\n  method: get\n  operationId: get_settings_integrations__integration_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/integrations/{integration_id}\n  method: delete\n  operationId: delete_settings_integrations__integration_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/integrations/{integration_id}\n  method: patch\n  operationId: patch_settings_integrations__integration_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/sites\n  method: post\n  operationId: post_settings_sites_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/sites\n\
  \  method: get\n  operationId: get_settings_sites_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/sites/{site_id}\n  method: delete\n  operationId: delete_settings_sites__site_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/sites/{site_id}\n  method: get\n  operationId: get_settings_sites__site_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/sites/{site_id}\n  method: patch\n  operationId: patch_settings_sites__site_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/agentic-access/armis-agentic-access.yml
summary_line: 34 operations · 17 acting · 1 human-in-the-loop
tags:
- Company
- Defense Government
- Security
- Cybersecurity
- Asset Intelligence
- Exposure Management
- IoT
- OT Security
- Vulnerability Management
- Developer Tools
---
