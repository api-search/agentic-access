---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 20
api_specs:
- filename: pterodactyl-admin-api-openapi.yml
  format: yaml
  label: Pterodactyl Admin API
  slug: pterodactyl-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-admin-api-openapi.yml
- filename: pterodactyl-application-api-openapi.yml
  format: yaml
  label: Pterodactyl Application API
  slug: pterodactyl-application-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-application-api-openapi.yml
- filename: pterodactyl-client-api-openapi.yml
  format: yaml
  label: Pterodactyl Client API
  slug: pterodactyl-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-client-api-openapi.yml
- filename: pterodactyl-gpg-api-openapi.yml
  format: yaml
  label: Pterodactyl Gpg API
  slug: pterodactyl-gpg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-gpg-api-openapi.yml
- filename: pterodactyl-installer-api-openapi.yml
  format: yaml
  label: Pterodactyl Installer API
  slug: pterodactyl-installer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-installer-api-openapi.yml
- filename: pterodactyl-pterodactyl-api-api-openapi.yml
  format: yaml
  label: Pterodactyl Pterodactyl API
  slug: pterodactyl-pterodactyl-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-pterodactyl-api-api-openapi.yml
- filename: pterodactyl-pterodactyl-api-openapi.yml
  format: yaml
  label: Pterodactyl Pterodactyl API
  slug: pterodactyl-pterodactyl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-pterodactyl-api-openapi.yml
- filename: pterodactyl-setup-22-api-openapi.yml
  format: yaml
  label: Pterodactyl Setup 22 API
  slug: pterodactyl-setup-22-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-setup-22-api-openapi.yml
consequence_counts:
  physical: 1
  read: 20
  safety-critical: 2
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Pterodactyl Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/extensions/architecto/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/users/1/disable-2fa
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/admin/nodes/1/deploy-token
operation_count: 33
overview: 'Pterodactyl exposes 33 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 10 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pterodactyl
provider_slug: pterodactyl
slug: pterodactyl-agentic-access
source_filename: pterodactyl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/pterodactyl-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 20\n    acting: 13\n  by_consequence:\n    read: 20\n    write: 10\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/extensions\n  method: get\n  operationId: get_api_admin_extensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/admin/extensions\n  method: post\n  operationId: post_api_admin_extensions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/extensions/architecto\n  method: delete\n  operationId: delete_api_admin_extensions_architecto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/extensions/architecto/disable\n  method: post\n  operationId: post_api_admin_extensions_architecto_disable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/extensions/architecto/enable\n  method: post\n  operationId: post_api_admin_extensions_architecto_enable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/extensions/architecto/settings\n  method: get\n  operationId: get_api_admin_extensions_architecto_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/extensions/architecto/settings\n  method: patch\n  operationId: patch_api_admin_extensions_architecto_settings\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/languages\n  method: get\n  operationId: get_api_admin_languages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/nodes/1/deploy-token\n  method: post\n  operationId: post_api_admin_nodes_1_deploy_token\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/nodes/1/system-information\n  method:\
  \ get\n  operationId: get_api_admin_nodes_1_system_information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/nodes/1/utilization\n  method: get\n  operationId: get_api_admin_nodes_1_utilization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/servers\n  method: get\n  operationId: get_api_admin_servers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/servers\n  method: post\n  operationId: post_api_admin_servers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/admin/servers/1/mounts\n  method: get\n  operationId: get_api_admin_servers_1_mounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/servers/1/mounts\n  method: post\n  operationId: post_api_admin_servers_1_mounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/servers/1/mounts/1\n  method: delete\n  operationId: delete_api_admin_servers_1_mounts_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/admin/servers/external/external-identifier\n  method: get\n  operationId: get_api_admin_servers_external_external_identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/users\n  method: get\n  operationId: get_api_admin_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/users\n  method: post\n  operationId: post_api_admin_users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/users/1\n  method: delete\n  operationId: delete_api_admin_users_1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/users/1\n  method: get\n  operationId: get_api_admin_users_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/users/1\n  method: put\n  operationId: put_api_admin_users_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/users/1/disable-2fa\n  method: post\n  operationId: post_api_admin_users_1_disable_2fa\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/users/external/external-identifier\n  method: get\n  operationId: get_api_admin_users_external_external_identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/application/users\n  method: get\n  operationId: get_api_application_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/client\n  method: get\n  operationId: get_api_client\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /gpg\n  method: get\n  operationId: get_gpg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installer\n  method: get\n  operationId: get_installer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pterodactyl/panel/releases/download/{downloadid}/panel.tar.gz\n  method: get\n  operationId: get_pterodactyl_panel_releases_download_downloadid_panel_tar_gz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pterodactyl/panel/releases/latest/download/panel.tar.gz\n  method: get\n  operationId: get_pterodactyl_panel_releases_latest_download_panel_tar_gz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /pterodactyl/wings/releases/latest/download/wings_linux_$([[\n  method: get\n  operationId: get_pterodactyl_wings_releases_latest_download_wings_linux\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setup_22.x\n  method: get\n  operationId: get_setup_22_x\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/pterodactyl/agentic-access/pterodactyl-agentic-access.yml
summary_line: 33 operations · 13 acting · 2 human-in-the-loop
tags:
- Company
- Game Server
- Open Source
- Docker
---
