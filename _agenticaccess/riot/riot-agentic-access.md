---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 31
api_specs:
- filename: riot-awareness-api-openapi.yml
  format: yaml
  label: Riot Awareness API
  slug: riot-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-awareness-api-openapi.yml
- filename: riot-breaches-api-openapi.yml
  format: yaml
  label: Riot Breaches API
  slug: riot-breaches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-breaches-api-openapi.yml
- filename: riot-general-api-openapi.yml
  format: yaml
  label: Riot General API
  slug: riot-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-general-api-openapi.yml
- filename: riot-groups-api-openapi.yml
  format: yaml
  label: Riot Groups API
  slug: riot-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-groups-api-openapi.yml
- filename: riot-inbox-api-openapi.yml
  format: yaml
  label: Riot Inbox API
  slug: riot-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-inbox-api-openapi.yml
- filename: riot-scim-api-openapi.yml
  format: yaml
  label: Riot SCIM API
  slug: riot-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-scim-api-openapi.yml
- filename: riot-simulation-api-openapi.yml
  format: yaml
  label: Riot Simulation API
  slug: riot-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-simulation-api-openapi.yml
- filename: riot-slash-api-openapi.yml
  format: yaml
  label: Riot Slash API
  slug: riot-slash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-slash-api-openapi.yml
- filename: riot-sonar-api-openapi.yml
  format: yaml
  label: Riot Sonar API
  slug: riot-sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-sonar-api-openapi.yml
consequence_counts:
  read: 31
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Riot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Riot exposes 40 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Riot
provider_slug: riot
slug: riot-agentic-access
source_filename: riot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/riot-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 31\n    acting: 9\n  by_consequence:\n    read: 31\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /scim/{workspace_id}/v2/Groups\n  method: get\n  operationId: groups_list_groups_ZC2NT5A\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Groups\n  method: post\n  operationId: groups_create_group_ZC2NT5A\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/Groups/{group_id}\n  method: delete\n  operationId: groups_delete_group_ZC2NT5A\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/Groups/{group_id}\n  method: get\n  operationId: groups_get_group_ZC2NT5A\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Groups/{group_id}\n  method: patch\n  operationId: groups_patch_group_ZC2NT5A\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/Groups/{group_id}\n  method: put\n  operationId: groups_update_group_ZC2NT5A\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/ResourceTypes\n  method: get\n  operationId: resource_types_list_resource_types_KKPMSEY\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /scim/{workspace_id}/v2/ResourceTypes/{resource_type_id}\n  method: get\n  operationId: resource_types_get_resource_type_KKPMSEY\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Schemas\n  method: get\n  operationId: schemas_list_schemas_DEOEZDI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Schemas/{schema}\n  method: get\n  operationId: schemas_get_schema_DEOEZDI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/ServiceProviderConfiguration\n  method: get\n  operationId: service_provider_configuration_get_service_provider_configuration_M4XZ6RY\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Users\n  method: get\n  operationId: users_list_users_3IQ5M4I\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Users\n  method: post\n  operationId: users_create_user_3IQ5M4I\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/Users/{user_id}\n  method: delete\n  operationId: users_delete_user_3IQ5M4I\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/Users/{user_id}\n  method: get\n  operationId: users_get_user_3IQ5M4I\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - scim:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/{workspace_id}/v2/Users/{user_id}\n  method: patch\n  operationId: users_patch_user_3IQ5M4I\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/{workspace_id}/v2/Users/{user_id}\n\
  \  method: put\n  operationId: users_update_user_3IQ5M4I\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - scim:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attack_login_domains\n  method: get\n  operationId: attack_login_domains_get_attack_login_domain_paginated_XU5W4YI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - simulation:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/breaches\n  method: get\n  operationId: breaches_get_paginated_FAUE35Y\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - breaches:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/breaches/statistics\n  method: get\n  operationId:\
  \ breaches_get_statistics_FAUE35Y\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - breaches:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/breaches/{breach_id}/compromised-employees\n  method: get\n  operationId: breaches_get_breach_compromised_employees_FAUE35Y\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - breaches:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns\n  method: get\n  operationId: campaigns_get_paginated_CWCTX3I\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - simulation:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/statistics\n  method: get\n  operationId: campaigns_get_statistics_CWCTX3I\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - simulation:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{campaign_id}/attacks\n  method: get\n  operationId: attacks_get_paginated_KCLEOEQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - simulation:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/courses\n  method: get\n  operationId: courses_get_paginated_DJESCNQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - awareness:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/courses/employees_progress\n  method: get\n  operationId: courses_get_employees_progress_DJESCNQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - awareness:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/courses/statistics\n  method: get\n  operationId: courses_get_statistics_DJESCNQ\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - awareness:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/courses/{course_id}\n  method: get\n  operationId: courses_get_course_statuses_of_employees_DJESCNQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - awareness:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n  method: get\n  operationId: domains_get_paginated_domains_OOWLIAA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email_reports/report_attack_from_message_id\n  method: post\n  operationId: reports_report_attack_from_message_id_DO4XYPA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - inbox:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employees\n  method: get\n  operationId: employees_get_paginated_LRY7OLI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employees/statistics\n  method: get\n  operationId: employees_get_statistics_LRY7OLI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employees/{employee_id}\n  method: get\n  operationId: employees_get_LRY7OLI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace:read\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/groups\n  method: get\n  operationId: groups_get_paginated_BOILCUA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - groups:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/groups/{group_id}/employees\n  method: get\n  operationId: groups_get_group_employees_BOILCUA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - groups:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inbox_tickets/list_employees_with_email_reports\n  method: get\n  operationId: inbox_tickets_list_employees_with_email_reports_QHKH7RI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inbox:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inbox_tickets/statistics\n  method: get\n  operationId: inbox_tickets_get_inbox_statistics_QHKH7RI\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inbox:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization\n  method: get\n  operationId: organizations_get_XEBQFJQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/slash/employees/alert_statistics\n  method: get\n  operationId: inbound_protections_list_employees_with_alerts_stats_YGL572Y\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inbox:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/slash/employees/impersonation_statistics\n  method: get\n  operationId: inbound_protections_list_employees_with_impersonation_stats_YGL572Y\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - inbox:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/agentic-access/riot-agentic-access.yml
summary_line: 40 operations · 9 acting
tags:
- Cybersecurity
- security-awareness
- human-risk-management
- phishing-simulation
- employee-security
- security-posture-management
- breach-detection
- email-security
- saas-security
- SCIM
- Webhook
- ocsf
- france
---
