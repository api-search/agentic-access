---
acting_count: 93
action_class_counts:
  acting: 93
  connected: 100
api_specs:
- filename: bugsnag-builds-api-openapi.yml
  format: yaml
  label: bugsnag Builds API
  slug: bugsnag-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-builds-api-openapi.yml
- filename: bugsnag-collaborators-api-openapi.yml
  format: yaml
  label: bugsnag Collaborators API
  slug: bugsnag-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-collaborators-api-openapi.yml
- filename: bugsnag-comments-api-openapi.yml
  format: yaml
  label: bugsnag Comments API
  slug: bugsnag-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-comments-api-openapi.yml
- filename: bugsnag-errors-api-openapi.yml
  format: yaml
  label: bugsnag Errors API
  slug: bugsnag-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-errors-api-openapi.yml
- filename: bugsnag-eventfields-api-openapi.yml
  format: yaml
  label: bugsnag EventFields API
  slug: bugsnag-eventfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-eventfields-api-openapi.yml
- filename: bugsnag-events-api-openapi.yml
  format: yaml
  label: bugsnag Events API
  slug: bugsnag-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-events-api-openapi.yml
- filename: bugsnag-organizations-api-openapi.yml
  format: yaml
  label: bugsnag Organizations API
  slug: bugsnag-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-organizations-api-openapi.yml
- filename: bugsnag-pivots-api-openapi.yml
  format: yaml
  label: bugsnag Pivots API
  slug: bugsnag-pivots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-pivots-api-openapi.yml
- filename: bugsnag-projects-api-openapi.yml
  format: yaml
  label: bugsnag Projects API
  slug: bugsnag-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-projects-api-openapi.yml
- filename: bugsnag-releases-api-openapi.yml
  format: yaml
  label: bugsnag Releases API
  slug: bugsnag-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-releases-api-openapi.yml
- filename: bugsnag-sessions-api-openapi.yml
  format: yaml
  label: bugsnag Sessions API
  slug: bugsnag-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-sessions-api-openapi.yml
- filename: bugsnag-stability-api-openapi.yml
  format: yaml
  label: bugsnag Stability API
  slug: bugsnag-stability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-stability-api-openapi.yml
- filename: bugsnag-traces-api-openapi.yml
  format: yaml
  label: bugsnag Traces API
  slug: bugsnag-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-traces-api-openapi.yml
- filename: bugsnag-trends-api-openapi.yml
  format: yaml
  label: bugsnag Trends API
  slug: bugsnag-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-trends-api-openapi.yml
- filename: bugsnag-current-user-api-openapi.yml
  format: yaml
  label: Bugsnag Current User API
  slug: bugsnag-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-current-user-api-openapi.yml
- filename: bugsnag-error-reporting-api-openapi.json
  format: json
  label: BugSnag Error Reporting API
  slug: bugsnag-error-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-error-reporting-api-openapi.json
- filename: bugsnag-upload-api-openapi.json
  format: json
  label: BugSnag Upload API
  slug: bugsnag-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-upload-api-openapi.json
consequence_counts:
  physical: 8
  read: 100
  safety-critical: 2
  write: 83
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Bugsnag Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /organizations/{id}/api_key
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /organizations/{id}/auth_token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organizations/{organization_id}/collaborators/{id}/team_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /organizations/{organization_id}/collaborators/{id}/team_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organizations/{organization_id}/teams/{id}/team_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /organizations/{organization_id}/teams/{id}/team_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /traces/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/traces
operation_count: 193
overview: 'Bugsnag exposes 193 API operations that an AI agent could call, of which 93 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 100 read, 83 write, 8 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bugsnag
provider_slug: bugsnag
slug: bugsnag-agentic-access
source_filename: bugsnag-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/bugsnag-build-api-openapi.json, openapi/bugsnag-builds-api-openapi.yml, openapi/bugsnag-collaborators-api-openapi.yml,\n  openapi/bugsnag-comments-api-openapi.yml, openapi/bugsnag-current-user-api-openapi.yml, openapi/bugsnag-data-access-api-openapi.json,\n  openapi/bugsnag-error-reporting-api-openapi.json, openapi/bugsnag-errors-api-openapi.yml,\n  openapi/bugsnag-eventfields-api-openapi.yml, openapi/bugsnag-events-api-openapi.yml, openapi/bugsnag-organizations-api-openapi.yml,\n  openapi/bugsnag-pivots-api-openapi.yml, openapi/bugsnag-projects-api-openapi.yml, openapi/bugsnag-releases-api-openapi.yml,\n  openapi/bugsnag-session-tracking-api-openapi.json, openapi/bugsnag-sessions-api-openapi.yml,\n  openapi/bugsnag-stability-api-openapi.yml, openapi/bugsnag-trace-api-openapi.json, openapi/bugsnag-traces-api-openapi.yml,\n  openapi/bugsnag-trends-api-openapi.yml, openapi/bugsnag-upload-api-openapi.json\ndescription:\
  \ Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 193\n  by_action_class:\n    acting: 93\n    connected: 100\n  by_consequence:\n    write: 83\n    read: 100\n    safety-critical: 2\n    physical: 8\n  human_in_the_loop_required: 2\noperations:\n- path: /\n  method: post\n  operationId: Notify of a build\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: createBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators\n  method: get\n  operationId: listOrganizationCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators\n  method: post\n  operationId: inviteOrganizationCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators/{collaborator_id}\n  method: get\n  operationId: getOrganizationCollaborator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{collaborator_id}\n  method: patch\n  operationId: updateOrganizationCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators/{collaborator_id}\n  method: delete\n  operationId: removeOrganizationCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}/comments\n  method: get\n  operationId: listErrorComments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}/comments\n  method: post\n  operationId: createErrorComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}/comments/{comment_id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}/comments/{comment_id}\n  method: patch\n  operationId: updateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}/comments/{comment_id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/organizations\n  method: get\n  operationId: listUserOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /projects/{project_id}/saved_searches\n  method: get\n  operationId: listProjectSavedSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saved_searches\n  method: post\n  operationId: createSavedSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved_searches/{id}\n  method: get\n  operationId: getSavedSearchById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saved_searches/{id}\n  method: patch\n  operationId: updateSavedSearchById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved_searches/{id}\n  method: delete\n  operationId: deleteSavedSearchById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved_searches/{id}/usage_summary\n  method: get\n  operationId: getSavedSearchUsageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/projects\n  method: get\n  operationId: getOrganizationProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/projects\n  method: post\n  operationId: createOrganizationProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors\n  method: get\n  operationId: listProjectErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors\n  method: patch\n  operationId: bulkUpdateErrors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors\n  method: delete\n  operationId: deleteAllErrorsInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}\n  method: get\n  operationId: viewErrorOnProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}\n  method: patch\n  operationId: updateErrorOnProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}\n  method: delete\n  operationId: deleteErrorOnProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/events/{event_id}\n  method: get\n  operationId: viewEventById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/events/{event_id}\n  method: delete\n  operationId: deleteEventById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}/events\n  method: get\n  operationId: listEventsOnError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /errors/{error_id}/latest_event\n  method: get\n  operationId: viewLatestEventOnError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/events\n  method: get\n  operationId: listEventsOnProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}/trends\n  method: get\n  operationId: getBucketedAndUnbucketedTrendsOnError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/trends\n  method: get\n  operationId: getBucketedAndUnbucketedTrendsOnProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}/pivots\n  method: get\n  operationId: listPivotsOnAnError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}/pivots/{event_field_display_id}/values\n  method: get\n  operationId: getPivotValuesOnAnError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/pivots\n  method: get\n  operationId: getPivotsOnAProject\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/pivots/{event_field_display_id}/values\n  method: get\n  operationId: getPivotValuesOnAProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments/{comment_id}\n  method: patch\n  operationId: updateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments/{comment_id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/errors/{error_id}/comments\n  method: get\n  operationId: listCommentsOnError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/errors/{error_id}/comments\n  method: post\n  operationId: createCommentOnError\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations\n  method: get\n  operationId: getIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/test\n  method: post\n  operationId: integrationsTest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configured_integrations/{id}\n  method: get\n  operationId: configuredIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configured_integrations/{id}\n  method: patch\n  operationId: configuredIntegrationsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configured_integrations/{id}\n  method: delete\n  operationId: configuredIntegrationsDelete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configured_integrations/{id}/trigger_configs/{trigger_config_key}\n  method: patch\n  operationId: updateConfiguredIntegrationsTriggerConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configured_integrations/{id}/test\n  method: post\n  operationId: configuredIntegrationTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/configured_integrations\n  method: post\n  operationId: projectConfiguredIntegrations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/configured_integration_summaries\n  method: get\n  operationId: projectConfiguredIntegrationSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/integration_connections\n  method: get\n  operationId: listOrganizationIntegrationConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /organizations\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}\n  method: get\n  operationId: getOrganizationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}\n  method: patch\n  operationId: updateOrganizationById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}\n  method: delete\n\
  \  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/api_key\n  method: delete\n  operationId: revokeOrganizationApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations/{id}/auth_token\n  method: delete\n  operationId: revokeOrganizationAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations/{organization_id}/collaborators\n  method: get\n  operationId: listOrganizationCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators\n  method: post\n  operationId: inviteOrganizationCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators/{id}\n  method: get\n  operationId: getOrganizationCollaborator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{id}\n  method: patch\n  operationId: updateOrganizationCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators/{id}\n  method: delete\n  operationId: deleteOrganizationCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators/bulk_invite\n  method: post\n  operationId: bulkInviteOrganizationCollaborators\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/collaborators\n  method: get\n  operationId: listProjectCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/collaborators/{id}\n  method: get\n  operationId: getProjectCollaborator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/project_access_counts\n  method: get\n  operationId: getOrganizationCollaboratorProjectAccessCounts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{collaborator_id}/projects\n  method: get\n  operationId: getOrganizationCollaboratorProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{collaborator_id}/project_accesses\n  method: get\n  operationId: listOrganizationCollaboratorProjectAccesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{collaborator_id}/project_accesses/{project_id}\n  method: get\n  operationId: getOrganizationCollaboratorProjectAccessById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /organizations/{organization_id}/collaborators/{id}/team_memberships\n  method: post\n  operationId: addOrganizationCollaboratorTeamMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/collaborators/{id}/team_memberships\n  method: delete\n  operationId: deleteOrganizationCollaboratorTeamMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /organizations/{organization_id}/teams\n  method: get\n  operationId: listOrganizationTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/teams\n  method: post\n  operationId: createOrganizationTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}\n  method: get\n  operationId: getOrganizationTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/teams/{id}\n  method: patch\n  operationId: updateOrganizationTeam\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}\n  method: delete\n  operationId: deleteOrganizationTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}/suggested_collaborators\n  method: get\n  operationId: listOrganizationTeamSuggestedCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{id}/teams\n\
  \  method: get\n  operationId: listOrganizationCollaboratorTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/collaborators/{id}/suggested_teams\n  method: get\n  operationId: listOrganizationCollaboratorSuggestedTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/teams/{id}/collaborators\n  method: get\n  operationId: listOrganizationTeamCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/teams/{id}/team_memberships\n  method: post\n  operationId: addOrganizationTeamMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}/team_memberships\n  method: delete\n  operationId: deleteOrganizationTeamMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}/project_accesses\n  method: get\n  operationId: listOrganizationTeamProjectAccesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /organizations/{organization_id}/teams/{id}/project_accesses\n  method: patch\n  operationId: updateOrganizationTeamProjectAccesses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}/project_accesses\n  method: delete\n  operationId: deleteOrganizationTeamProjectAccesses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/teams/{id}/suggested_projects\n  method: get\n  operationId: listOrganizationTeamSuggestedProjects\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/event_data_requests\n  method: post\n  operationId: organizationEventDataRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/event_data_requests/{id}\n  method: get\n  operationId: organizationEventDataRequestsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/event_data_deletions\n  method: post\n  operationId: organizationEventDataDeletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/event_data_deletions/{id}/confirm\n  method: post\n  operationId: organizationEventDataDeletionsConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/event_data_deletions/{id}\n  method: get\n  operationId: organizationEventDataDeletionsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/scim/v2/Users\n  method: get\n  operationId: listScimCollaborators\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/scim/v2/Users\n  method: post\n  operationId: createScimCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/scim/v2/Users/{id}\n  method: get\n  operationId: getScimCollaborator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/scim/v2/Users/{id}\n  method: put\n  operationId: updateScimCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/scim/v2/Users/{id}\n  method: patch\n  operationId: patchScimCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/scim/v2/Users/{id}\n  method: delete\n  operationId: deleteScimCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/scim\n\
  \n# --- truncated at 32 KB (58 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/agentic-access/bugsnag-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/agentic-access/bugsnag-agentic-access.yml
summary_line: 193 operations · 93 acting · 2 human-in-the-loop
tags:
- Monitoring
- Observability
- Error Monitoring
- Application Performance Monitoring
- Distributed Tracing
- Developer Tools
- SmartBear
---
