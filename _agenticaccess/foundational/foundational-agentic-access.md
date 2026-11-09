---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 15
api_specs:
- filename: foundational-auth-api-openapi.yml
  format: yaml
  label: Foundational Auth API
  slug: foundational-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-auth-api-openapi.yml
- filename: foundational-lineage-api-openapi.yml
  format: yaml
  label: Foundational Lineage API
  slug: foundational-lineage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-lineage-api-openapi.yml
- filename: foundational-manual-lineage-api-openapi.yml
  format: yaml
  label: Foundational Manual Lineage API
  slug: foundational-manual-lineage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-manual-lineage-api-openapi.yml
- filename: foundational-monitors-api-openapi.yml
  format: yaml
  label: Foundational Monitors API
  slug: foundational-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-monitors-api-openapi.yml
- filename: foundational-onboarding-api-openapi.yml
  format: yaml
  label: Foundational Onboarding API
  slug: foundational-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-onboarding-api-openapi.yml
- filename: foundational-policies-api-openapi.yml
  format: yaml
  label: Foundational Policies API
  slug: foundational-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-policies-api-openapi.yml
consequence_counts:
  read: 15
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Foundational Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'Foundational exposes 34 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Foundational
provider_slug: foundational
slug: foundational-agentic-access
source_filename: foundational-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/foundational-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 19\n    connected: 15\n  by_consequence:\n    write: 19\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/api-token\n  method: post\n  operationId: exchange_client_credentials_for_access_token_auth_api_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/search\n  method: get\n  operationId: search_for_entities_lineage_search_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/dashboards/usage-ranking\n  method: get\n  operationId: rank_dashboards_by_usage_lineage_dashboards_usage_ranking_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/pr/issues/diff\n  method: get\n  operationId: get_pr_diff_lineage_pr_issues_diff_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/pr/issues\n  method: get\n  operationId: get_pr_issues_lineage_pr_issues_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/entity/{entity_id}\n  method: get\n  operationId: get_entity_and_its_dependencies_lineage_entity__entity_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/entity/{entity_id}/triggers\n  method: get\n  operationId: get_operation_triggers_lineage_entity__entity_id__triggers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/entity/{entity_id}/triggered-by\n  method: get\n  operationId: get_operation_triggered_by_lineage_entity__entity_id__triggered_by_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/edge/{source_id}/{dest_id}/{edge_type}/provenance\n  method: get\n  operationId: get_edge_provenance_lineage_edge__source_id___dest_id___edge_type__provenance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/entity/{entity_id}/neighbors\n  method: get\n  operationId: get_app_graph_neighbors_lineage_entity__entity_id__neighbors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lineage/entity/{entity_id}/tags\n  method: post\n  operationId: set_entity_tags_lineage_entity__entity_id__tags_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/entity/{entity_id}/tags/{tag_name}\n  method: delete\n  operationId: delete_entity_tag_lineage_entity__entity_id__tags__tag_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/entity/{entity_id}/certification\n  method: put\n  operationId: set_entity_certification_lineage_entity__entity_id__certification_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/entity/{entity_id}/certification\n  method: delete\n  operationId: clear_entity_certification_lineage_entity__entity_id__certification_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /lineage/entity/{entity_id}/description\n  method: put\n  operationId: set_entity_description_lineage_entity__entity_id__description_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/entity/{entity_id}/description\n  method: delete\n  operationId: clear_entity_description_lineage_entity__entity_id__description_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/entity/{entity_id}/{direction}\n  method: get\n  operationId: get_entity_dependencies_lineage_entity__entity_id___direction__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/repos\n  method: get\n  operationId: list_org_repos_onboarding_repos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/repos/{repo_name}/trigger\n  method: post\n  operationId: trigger_repo_onboarding_onboarding_repos__repo_name__trigger_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarding/repos/{repo_name}\n  method: delete\n  operationId: offboard_repo_onboarding_repos__repo_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarding/powerbi/workspaces\n  method: get\n  operationId: list_powerbi_workspaces_onboarding_powerbi_workspaces_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/powerbi/workspaces\n  method: post\n  operationId: add_powerbi_workspace_onboarding_powerbi_workspaces_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarding/powerbi/workspaces/{workspace_id}\n  method: delete\n  operationId: remove_powerbi_workspace_onboarding_powerbi_workspaces__workspace_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/issue-types\n  method: get\n  operationId: list_issue_types_policies_issue_types_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies\n  method: get\n  operationId: list_policies_policies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies\n  method: post\n  operationId: create_policy_policies_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/{policy_id}\n  method: get\n  operationId: get_policy_policies__policy_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies/{policy_id}\n  method: patch\n  operationId: update_policy_policies__policy_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/{policy_id}\n  method: delete\n  operationId: delete_policy_policies__policy_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manual-lineage/snapshot\n  method: post\n  operationId: create_manual_lineage_snapshot_manual_lineage_snapshot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manual-lineage/connectors/{connector_id}/snapshot\n  method: post\n  operationId: ingest_manual_lineage_snapshot_manual_lineage_connectors__connector_id__snapshot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manual-lineage/connectors/{connector_id}\n\
  \  method: put\n  operationId: rename_manual_lineage_connector_manual_lineage_connectors__connector_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/preview\n  method: post\n  operationId: preview_monitor_monitors_preview_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/custom-queries\n  method: put\n  operationId: upsert_custom_query_monitor_monitors_custom_queries_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/foundational/agentic-access/foundational-agentic-access.yml
summary_line: 34 operations · 19 acting
tags:
- Company
- Data Governance
- Artificial Intelligence
- Data Management
- Data Lineage
---
