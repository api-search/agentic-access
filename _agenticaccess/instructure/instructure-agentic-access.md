---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 18
api_specs:
- filename: instructure-externaltool-api-openapi.yml
  format: yaml
  label: Instructure ExternalTool API
  slug: instructure-externaltool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-externaltool-api-openapi.yml
- filename: instructure-lti-accountexternaltool-api-openapi.yml
  format: yaml
  label: Instructure Lti::AccountExternalTool API
  slug: instructure-lti-accountexternaltool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-accountexternaltool-api-openapi.yml
- filename: instructure-lti-accountlookup-api-openapi.yml
  format: yaml
  label: Instructure Lti::AccountLookup API
  slug: instructure-lti-accountlookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-accountlookup-api-openapi.yml
- filename: instructure-lti-dataservice-api-openapi.yml
  format: yaml
  label: Instructure Lti::DataService API
  slug: instructure-lti-dataservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-dataservice-api-openapi.yml
- filename: instructure-lti-ims-authentication-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::Authentication API
  slug: instructure-lti-ims-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-authentication-api-openapi.yml
- filename: instructure-lti-ims-dynamicregistration-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::DynamicRegistration API
  slug: instructure-lti-ims-dynamicregistration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-dynamicregistration-api-openapi.yml
- filename: instructure-lti-ims-lineitem-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::LineItem API
  slug: instructure-lti-ims-lineitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-lineitem-api-openapi.yml
- filename: instructure-lti-ims-namesandrole-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::NamesAndRole API
  slug: instructure-lti-ims-namesandrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-namesandrole-api-openapi.yml
- filename: instructure-lti-ims-result-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::Result API
  slug: instructure-lti-ims-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-result-api-openapi.yml
- filename: instructure-lti-membershipservice-api-openapi.yml
  format: yaml
  label: Instructure Lti::MembershipService API
  slug: instructure-lti-membershipservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-membershipservice-api-openapi.yml
- filename: instructure-lti-toolconfigurationsapi-api-openapi.yml
  format: yaml
  label: Instructure Lti::ToolConfigurationsApi API
  slug: instructure-lti-toolconfigurationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-toolconfigurationsapi-api-openapi.yml
- filename: instructure-security-api-openapi.yml
  format: yaml
  label: Instructure Security API
  slug: instructure-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-security-api-openapi.yml
consequence_counts:
  read: 18
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Instructure Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Instructure exposes 23 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Instructure
provider_slug: instructure
slug: instructure-agentic-access
source_filename: instructure-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/instructure-canvas-lti-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 18\n    acting: 5\n  by_consequence:\n    read: 18\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/lti/accounts/{account_id}/data_services\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/accounts/{account_id}/data_services/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/accounts/{account_id}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/accounts/{account_id}/external_tools\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/accounts/{account_id}/external_tools/{external_tool_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/accounts/{account_id}/developer_keys/tool_configuration\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lti/accounts/{account_id}/developer_keys/{developer_key_id}/tool_configuration\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/authorize_redirect\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lti/courses/{course_id}/line_items\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/courses/{course_id}/names_and_roles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/courses/{course_id}/line_items/{line_item_id}/results\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/courses/{course_id}/line_items/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/courses/{course_id}/line_items/{line_item_id}/results/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/courses/{course_id}/jwt_token\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/developer_keys/{developer_key_id}/tool_configuration\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lti/developer_keys/{developer_key_id}/tool_configuration\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lti/groups/{group_id}/names_and_roles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/groups/{group_id}/membership_service\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/register\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/registration_token\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/registrations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lti/security/jwks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lti/security/openid-configuration\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/agentic-access/instructure-agentic-access.yml
summary_line: 23 operations · 5 acting
tags:
- EdTech
- Education
- LMS
- Canvas
- Courses
- Enrollments
- Assignments
- Grades
- Discussions
- GraphQL
- LTI
- Learning Management
---
