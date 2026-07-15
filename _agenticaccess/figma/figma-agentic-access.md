---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 25
api_specs:
- filename: figma-api-openapi.yml
  format: yaml
  label: Figma API
  slug: figma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma REST API
  slug: figma-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-files-api-openapi.yml
  format: yaml
  label: Figma Files API
  slug: figma-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-files-api-openapi.yml
- filename: figma-images-api-openapi.yml
  format: yaml
  label: Figma Images API
  slug: figma-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-images-api-openapi.yml
- filename: figma-teams-api-openapi.yml
  format: yaml
  label: Figma Teams API
  slug: figma-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-teams-api-openapi.yml
- filename: figma-projects-api-openapi.yml
  format: yaml
  label: Figma Projects API
  slug: figma-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-projects-api-openapi.yml
- filename: figma-me-api-openapi.yml
  format: yaml
  label: Figma Me API
  slug: figma-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-me-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Components API
  slug: figma-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-component-sets-api-openapi.yml
  format: yaml
  label: Figma Component Sets API
  slug: figma-component-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-component-sets-api-openapi.yml
- filename: figma-styles-api-openapi.yml
  format: yaml
  label: Figma Styles API
  slug: figma-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-styles-api-openapi.yml
- filename: figma-activity-logs-api-openapi.yml
  format: yaml
  label: Figma Activity Logs API
  slug: figma-activity-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-activity-logs-api-openapi.yml
- filename: figma-payments-api-openapi.yml
  format: yaml
  label: Figma Payments API
  slug: figma-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-payments-api-openapi.yml
- filename: figma-dev-resources-api-openapi.yml
  format: yaml
  label: Figma Dev Resources API
  slug: figma-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-dev-resources-api-openapi.yml
- filename: figma-analytics-api-openapi.yml
  format: yaml
  label: Figma Analytics API
  slug: figma-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-analytics-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Comments API
  slug: figma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Version History API
  slug: figma-version-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Variables API
  slug: figma-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Library Analytics API
  slug: figma-library-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
consequence_counts:
  read: 25
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Figma Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Figma exposes 31 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Figma
provider_slug: figma
slug: figma-agentic-access
source_filename: figma-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/figma-activity-logs-api-openapi.yml, openapi/figma-analytics-api-openapi.yml,\n  openapi/figma-api-openapi.yml, openapi/figma-component-sets-api-openapi.yml, openapi/figma-dev-resources-api-openapi.yml,\n  openapi/figma-files-api-openapi.yml, openapi/figma-images-api-openapi.yml, openapi/figma-me-api-openapi.yml,\n  openapi/figma-payments-api-openapi.yml, openapi/figma-projects-api-openapi.yml, openapi/figma-rest-api-openapi.yml,\n  openapi/figma-styles-api-openapi.yml, openapi/figma-teams-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 25\n    acting: 6\n  by_consequence:\n    read: 25\n    write: 6\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /v1/activity_logs\n  method: get\n  operationId: getActivityLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - org:activity_log_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/libraries/{file_key}/usages\n  method: get\n  operationId: getLibraryAnalyticsUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - library_analytics:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/component_sets/{key}\n  method: get\n  operationId: getComponentSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dev_resources\n  method: post\n  operationId: postDevResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - file_dev_resources:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dev_resources\n  method: put\n  operationId: putDevResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - file_dev_resources:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_key}/dev_resources/{dev_resource_id}\n  method: delete\n  operationId: deleteDevResource\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - file_dev_resources:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/{file_key}\n  method: get\n  operationId: getImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/files\n\
  \  method: get\n  operationId: getProjectFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/nodes\n  method: get\n  operationId: getFileNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/{file_key}\n  method: get\n  operationId: getImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/image_fills\n\
  \  method: get\n  operationId: getImageFills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/versions\n  method: get\n  operationId: getFileVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/comments\n  method: post\n  operationId: postComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - file_comments:write\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_key}/comments/{comment_id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - file_comments:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_key}/comments/{comment_id}/reactions\n  method: get\n  operationId: getCommentReactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/comments/{comment_id}/reactions\n  method: post\n  operationId: postCommentReaction\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - file_comments:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/teams/{team_id}/components\n  method: get\n  operationId: getTeamComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_key}/components\n  method: get\n  operationId: getFileComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{key}\n  method: get\n  operationId: getComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams/{team_id}/component_sets\n  method: get\n  operationId: getTeamComponentSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams/{team_id}/styles\n  method: get\n  operationId: getTeamStyles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams/{team_id}/projects\n  method: get\n  operationId: getTeamProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/files\n  method: get\n  operationId: getProjectFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/styles/{key}\n  method: get\n  operationId: getStyle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_id}/webhooks\n  method: get\n  operationId: getTeamWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - files:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/agentic-access/figma-agentic-access.yml
summary_line: 31 operations · 6 acting
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
---
