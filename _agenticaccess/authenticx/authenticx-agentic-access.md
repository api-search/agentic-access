---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 28
api_specs:
- filename: authenticx-agent-api-openapi.yml
  format: yaml
  label: Authenticx Agent API
  slug: authenticx-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-agent-api-openapi.yml
- filename: authenticx-conversations-api-openapi.yml
  format: yaml
  label: Authenticx Conversations API
  slug: authenticx-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-conversations-api-openapi.yml
- filename: authenticx-evaluations-api-openapi.yml
  format: yaml
  label: Authenticx Evaluations API
  slug: authenticx-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-evaluations-api-openapi.yml
- filename: authenticx-hierarchy-api-openapi.yml
  format: yaml
  label: Authenticx Hierarchy API
  slug: authenticx-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-hierarchy-api-openapi.yml
- filename: authenticx-interactions-api-openapi.yml
  format: yaml
  label: Authenticx Interactions API
  slug: authenticx-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-interactions-api-openapi.yml
- filename: authenticx-media-api-openapi.yml
  format: yaml
  label: Authenticx Media API
  slug: authenticx-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-media-api-openapi.yml
- filename: authenticx-metadata-api-openapi.yml
  format: yaml
  label: Authenticx Metadata API
  slug: authenticx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-metadata-api-openapi.yml
- filename: authenticx-modelresults-api-openapi.yml
  format: yaml
  label: Authenticx Model Results API
  slug: authenticx-modelresults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-modelresults-api-openapi.yml
- filename: authenticx-receipts-api-openapi.yml
  format: yaml
  label: Authenticx Receipts API
  slug: authenticx-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-receipts-api-openapi.yml
- filename: authenticx-roles-api-openapi.yml
  format: yaml
  label: Authenticx Roles API
  slug: authenticx-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-roles-api-openapi.yml
- filename: authenticx-scim-resourcetypes-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) ResourceTypes API
  slug: authenticx-scim-resourcetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-resourcetypes-api-openapi.yml
- filename: authenticx-scim-schemas-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) Schemas API
  slug: authenticx-scim-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-schemas-api-openapi.yml
- filename: authenticx-scim-serviceproviderconfig-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) ServiceProviderConfig API
  slug: authenticx-scim-serviceproviderconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-serviceproviderconfig-api-openapi.yml
- filename: authenticx-scim-users-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) Users API
  slug: authenticx-scim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-users-api-openapi.yml
- filename: authenticx-textmedia-api-openapi.yml
  format: yaml
  label: Authenticx Text Media API
  slug: authenticx-textmedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-textmedia-api-openapi.yml
- filename: authenticx-user-api-openapi.yml
  format: yaml
  label: Authenticx User API
  slug: authenticx-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-user-api-openapi.yml
- filename: authenticx-userhierarchy-api-openapi.yml
  format: yaml
  label: Authenticx User Hierarchy API
  slug: authenticx-userhierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-userhierarchy-api-openapi.yml
- filename: authenticx-workflows-api-openapi.yml
  format: yaml
  label: Authenticx Workflows API
  slug: authenticx-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-workflows-api-openapi.yml
consequence_counts:
  read: 28
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Authenticx Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 46
overview: 'Authenticx exposes 46 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Authenticx
provider_slug: authenticx
slug: authenticx-agentic-access
source_filename: authenticx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/authenticx-acxapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    acting: 18\n    connected: 28\n  by_consequence:\n    write: 18\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /Agent\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Agent/{AgentId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Agent/{AgentId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Agent/All\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Conversations/Classifiers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Conversations/Insights\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Conversations/Insights\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Conversations/Transcriptions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Conversations/Transcriptions/{conversationId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - acxapi\n- path: /Evaluations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Evaluations/Modules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Hierarchy\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Hierarchy/{HierarchyId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Hierarchy/All\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Interactions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Interactions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Interactions/{AmdID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Media/Upload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /Metadata\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Metadata\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    -\
  \ acxapi\n- path: /Metadata/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /ModelResults\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /ModelResults/Conversation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Receipts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path:\
  \ /Roles/All\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/ResourceTypes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/ResourceTypes/{ResourceTypeId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/Schemas\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/Schemas/{SchemaUri}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/ServiceProviderConfig\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/Users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/Users\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /scim/v2/Users/{UserId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /scim/v2/Users/{UserId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /scim/v2/Users/{UserId}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /scim/v2/Users/{UserId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /TextMedia/Upload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /User\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /User\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n  \
  \  scope:\n    - acxapi\n- path: /User/{UserId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /User/{UserId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /User/All\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /UserHierarchy/{UserId}/{HierarchyId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - acxapi\n- path: /UserHierarchy/{UserId}/{HierarchyId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - acxapi\n- path: /UserHierarchy/{UserId}/All\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n- path: /Workflows\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - acxapi\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/agentic-access/authenticx-agentic-access.yml
summary_line: 46 operations · 18 acting
tags:
- conversation-intelligence
- healthcare
- speech-analytics
- contact-center
- customer-experience
- quality-assurance
- pharmacovigilance
- patient-experience
- transcription
- life-sciences
- scim
- oauth2
---
