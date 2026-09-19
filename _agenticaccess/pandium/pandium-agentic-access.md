---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 15
api_specs:
- filename: pandium-connector-calls-api-openapi.yml
  format: yaml
  label: Pandium Connector Calls API
  slug: pandium-connector-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-connector-calls-api-openapi.yml
- filename: pandium-integrations-api-openapi.yml
  format: yaml
  label: Pandium Integrations API
  slug: pandium-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-integrations-api-openapi.yml
- filename: pandium-runs-api-openapi.yml
  format: yaml
  label: Pandium Runs API
  slug: pandium-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-runs-api-openapi.yml
- filename: pandium-tenant-metadata-api-openapi.yml
  format: yaml
  label: Pandium Tenant Metadata API
  slug: pandium-tenant-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-tenant-metadata-api-openapi.yml
- filename: pandium-tenants-api-openapi.yml
  format: yaml
  label: Pandium Tenants API
  slug: pandium-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-tenants-api-openapi.yml
- filename: pandium-builds-api-openapi.yml
  format: yaml
  label: Pandium Builds API
  slug: pandium-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-builds-api-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Pandium Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/sourcecontrol/build
operation_count: 29
overview: 'Pandium exposes 29 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 13 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pandium
provider_slug: pandium
slug: pandium-agentic-access
source_filename: pandium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/pandium-builds-api-openapi.yml, openapi/pandium-connector-calls-api-openapi.yml,\n  openapi/pandium-integrations-api-openapi.yml, openapi/pandium-runs-api-openapi.yml, openapi/pandium-tenant-metadata-api-openapi.yml,\n  openapi/pandium-tenants-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 14\n    connected: 15\n  by_consequence:\n    safety-critical: 1\n    write: 13\n    read: 15\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/sourcecontrol/build\n  method: post\n  operationId: create_build_v2_v2_sourcecontrol_build_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/tenants/{tenant_id}/connectors/{connector_name}/call\n  method: post\n  operationId: proxyConnectorCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/integrations\n  method: get\n  operationId: get_many_integrations_v2_integrations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/integrations/{integration_id}\n  method: get\n  operationId: get_one_integration_v2_integrations__integration_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/integrations/{integration_id}/releases\n  method: get\n  operationId: get_integration_releases_v2_integrations__integration_id__releases_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/integrations/{integration_id}/releases/default\n  method: get\n  operationId: get_default_integration_release_v2_integrations__integration_id__releases_default_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/integrations/{integration_id}/releases/latest\n  method: get\n  operationId: get_latest_release_v2_integrations__integration_id__releases_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/integrations/{integration_id}/releases/{release_id}\n  method: get\n  operationId: get_one_integration_release_v2_integrations__integration_id__releases__release_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/integrations/{integration_id}/sync\n  method: post\n  operationId: sync_by_integration_id_v2_integrations__integration_id__sync_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/runs/triggers/{trigger_id}/status\n  method: get\n  operationId: get_run_status_from_trigger_v2_runs_triggers__trigger_id__status_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/runs/{run_id}/log\n  method: get\n  operationId: get_run_log_v2_runs__run_id__log_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}/sync\n  method: post\n  operationId: triggerTenantSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/runs\n  method: get\n  operationId: listTenantRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}/runs/{trigger_id}\n  method: get\n\
  \  operationId: getRunByTriggerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}/metadata\n  method: get\n  operationId: getTenantMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}/metadata\n  method: patch\n  operationId: updateTenantMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants\n  method: get\n  operationId: get_many_tenants_v2_tenants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/tenants\n  method: post\n  operationId: create_one_v2_tenants_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}\n  method: delete\n  operationId: delete_tenant_v2_tenants__tenant_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}\n  method: get\n  operationId: getTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}\n\
  \  method: patch\n  operationId: updateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/connectors/{connector_name}/call\n  method: post\n  operationId: proxy_connector_call_rest_v2_tenants__tenant_id__connectors__connector_name__call_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/connectors/{connector_name}/disconnect\n  method: patch\n  operationId: disconnect_tenant_connector_v2_tenants__tenant_id__connectors__connector_name__disconnect_patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/connectors/{connector_name}/soap\n  method: post\n  operationId: proxy_connector_call_soap_v2_tenants__tenant_id__connectors__connector_name__soap_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/connectors/{connector_name}/xml\n  method: post\n  operationId: proxy_connector_call_xml_v2_tenants__tenant_id__connectors__connector_name__xml_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/metadata\n  method: get\n  operationId: get_metadata_v2_tenants__tenant_id__metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}/metadata\n  method: patch\n  operationId: patch_metadata_v2_tenants__tenant_id__metadata_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tenants/{tenant_id}/runs\n  method: get\n  operationId: get_tenant_runs_v2_tenants__tenant_id__runs_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tenants/{tenant_id}/sync\n  method: post\n  operationId: sync_by_tenant_id_v2_tenants__tenant_id__sync_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/agentic-access/pandium-agentic-access.yml
summary_line: 29 operations · 14 acting · 1 human-in-the-loop
tags:
- B2B
- Hub
- Integration
- Workflows
- iPaaS
---
