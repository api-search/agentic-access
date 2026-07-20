---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 12
api_specs:
- filename: ardent-openapi-original.json
  format: json
  label: Ardent API
  slug: ardent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ardent/refs/heads/main/openapi/ardent-openapi-original.json
consequence_counts:
  read: 12
  safety-critical: 2
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Ardent Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/orgs/{org_id}/api-keys/{api_key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/orgs/{org_id}/invites/{invite_id}
operation_count: 35
overview: 'Ardent exposes 35 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 21 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ardent
provider_slug: ardent
slug: ardent-agentic-access
source_filename: ardent-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/ardent-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 23\n    connected: 12\n  by_consequence:\n    write: 21\n    read: 12\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/branch/create\n  method: post\n  operationId: create_service_branch_v1_branch_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/branches/{connector_id}\n  method: get\n  operationId:\
  \ get_branches_v1_branches__connector_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connectors\n  method: get\n  operationId: list_connectors_endpoint_v1_connectors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connectors\n  method: post\n  operationId: create_connector_endpoint_v1_connectors_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/preflight\n  method: post\n  operationId: preflight_connector_endpoint_v1_connectors_preflight_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}\n  method: delete\n  operationId: delete_connector_endpoint_v1_connectors__connector_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}\n  method: get\n  operationId: get_connector_endpoint_v1_connectors__connector_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connectors/{connector_id}\n  method: put\n  operationId: update_connector_endpoint_v1_connectors__connector_id__put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}/deletion-lock\n  method: delete\n  operationId: unlock_connector_deletion_endpoint_v1_connectors__connector_id__deletion_lock_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}/deletion-lock\n  method: post\n  operationId: lock_connector_deletion_endpoint_v1_connectors__connector_id__deletion_lock_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}/discover\n  method: post\n  operationId: discover_connector_endpoint_v1_connectors__connector_id__discover_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}/engine-setup\n  method: post\n  operationId: engine_setup_endpoint_v1_connectors__connector_id__engine_setup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/connectors/{connector_id}/quarantine\n  method: get\n  operationId: list_connector_quarantines_endpoint_v1_connectors__connector_id__quarantine_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connectors/{connector_id}/quarantine/{quarantine_id}/release\n  method: post\n  operationId: release_quarantine_endpoint_v1_connectors__connector_id__quarantine__quarantine_id__release_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}/replica-identity-decisions\n  method: put\n  operationId: set_replica_identity_decisions_endpoint_v1_connectors__connector_id__replica_identity_decisions_put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connectors/{connector_id}/selection\n  method: post\n  operationId: set_selection_endpoint_v1_connectors__connector_id__selection_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/operations/{operation_id}\n  method: get\n  operationId: get_operation_endpoint_v1_operations__operation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs/{org_id}\n\
  \  method: delete\n  operationId: delete_org_v1_orgs__org_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orgs/{org_id}\n  method: get\n  operationId: get_org_details_v1_orgs__org_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs/{org_id}\n  method: patch\n  operationId: update_org_v1_orgs__org_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orgs/{org_id}/api-keys\n  method:\
  \ get\n  operationId: list_api_keys_v1_orgs__org_id__api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs/{org_id}/api-keys\n  method: post\n  operationId: create_new_api_key_v1_orgs__org_id__api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orgs/{org_id}/api-keys/{api_key_id}\n  method: delete\n  operationId: revoke_api_key_endpoint_v1_orgs__org_id__api_keys__api_key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/orgs/{org_id}/invite\n  method: post\n  operationId: invite_user_to_org_v1_orgs__org_id__invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orgs/{org_id}/invites\n  method: get\n  operationId: list_pending_invites_v1_orgs__org_id__invites_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs/{org_id}/invites/{invite_id}\n  method: delete\n  operationId: revoke_invite_v1_orgs__org_id__invites__invite_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/orgs/{org_id}/members\n  method: get\n  operationId: list_org_members_v1_orgs__org_id__members_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orgs/{org_id}/members/{target_user_id}\n  method: delete\n  operationId: remove_org_member_v1_orgs__org_id__members__target_user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orgs/{org_id}/members/{target_user_id}\n  method: patch\n  operationId: update_member_role_v1_orgs__org_id__members__target_user_id__patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orgs/{org_id}/roles\n  method: get\n  operationId: list_org_roles_v1_orgs__org_id__roles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects\n  method: get\n  operationId: list_projects_endpoint_v1_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects\n  method: post\n  operationId: create_project_endpoint_v1_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}\n  method: delete\n  operationId: delete_project_endpoint_v1_projects__project_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}\n  method: get\n  operationId: get_project_endpoint_v1_projects__project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}\n  method: patch\n  operationId: update_project_endpoint_v1_projects__project_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ardent/refs/heads/main/agentic-access/ardent-agentic-access.yml
summary_line: 35 operations · 23 acting · 2 human-in-the-loop
tags:
- Company
- Database
- PostgreSQL
- Database Branching
- Developer Tools
- Sandbox
- AI Agents
- CI/CD
- Data Infrastructure
- Testing
---
