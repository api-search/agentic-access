---
acting_count: 40
action_class_counts:
  acting: 40
  connected: 41
api_specs:
- filename: contraforce-agent-tools-api-openapi.yml
  format: yaml
  label: Contraforce Agent Tools API
  slug: contraforce-agent-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-agent-tools-api-openapi.yml
- filename: contraforce-azure-resources-api-openapi.yml
  format: yaml
  label: Contraforce Azure resources API
  slug: contraforce-azure-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-azure-resources-api-openapi.yml
- filename: contraforce-cross-workspace-data-sources-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace data sources API
  slug: contraforce-cross-workspace-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-data-sources-api-openapi.yml
- filename: contraforce-cross-workspace-gamebooks-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace gamebooks API
  slug: contraforce-cross-workspace-gamebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-gamebooks-api-openapi.yml
- filename: contraforce-cross-workspace-incidents-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace incidents API
  slug: contraforce-cross-workspace-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-incidents-api-openapi.yml
- filename: contraforce-data-sources-api-openapi.yml
  format: yaml
  label: Contraforce Data sources API
  slug: contraforce-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-data-sources-api-openapi.yml
- filename: contraforce-export-api-openapi.yml
  format: yaml
  label: Contraforce Export API
  slug: contraforce-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-export-api-openapi.yml
- filename: contraforce-gamebooks-api-openapi.yml
  format: yaml
  label: Contraforce Gamebooks API
  slug: contraforce-gamebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-gamebooks-api-openapi.yml
- filename: contraforce-incidents-api-openapi.yml
  format: yaml
  label: Contraforce Incidents API
  slug: contraforce-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-incidents-api-openapi.yml
- filename: contraforce-investigation-api-openapi.yml
  format: yaml
  label: Contraforce Investigation API
  slug: contraforce-investigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-investigation-api-openapi.yml
- filename: contraforce-service-accounts-api-openapi.yml
  format: yaml
  label: Contraforce Service accounts API
  slug: contraforce-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-service-accounts-api-openapi.yml
- filename: contraforce-service-tickets-api-openapi.yml
  format: yaml
  label: Contraforce Service tickets API
  slug: contraforce-service-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-service-tickets-api-openapi.yml
- filename: contraforce-users-api-openapi.yml
  format: yaml
  label: Contraforce Users API
  slug: contraforce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-users-api-openapi.yml
- filename: contraforce-webhooks-api-openapi.yml
  format: yaml
  label: Contraforce Webhooks API
  slug: contraforce-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 41
  safety-critical: 2
  write: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Contraforce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/service-accounts/{id}/credentials/{credentialId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/service-accounts/{id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/service-accounts/sentinel-ingest/deployment-card
operation_count: 81
overview: 'Contraforce exposes 81 API operations that an AI agent could call, of which 40 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read, 37 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Contraforce
provider_slug: contraforce
slug: contraforce-agentic-access
source_filename: contraforce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: generated\nsource: openapi/contraforce-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 81\n  by_action_class:\n    connected: 41\n    acting: 40\n  by_consequence:\n    read: 41\n    write: 37\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}\n  method: get\n  operationId: v2-get-incident-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/evidence\n  method: get\n  operationId: v2-get-incident-evidence\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/last-gamebook\n  method: get\n  operationId: v2-get-incident-last-gamebook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/by-entity\n  method: get\n  operationId: v2-get-incidents-by-entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/status\n  method: put\n  operationId: v2-update-incident-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/assignee\n  method: put\n  operationId: v2-assign-incident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/comments\n  method: get\n  operationId: v2-get-incident-comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/comments\n  method: post\n  operationId: v2-create-incident-comment\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/comments/{commentId}\n  method: put\n  operationId: v2-update-incident-comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/incidents/{source}/{incidentId}/comments/{commentId}\n  method: delete\n  operationId: v2-delete-incident-comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/incidents/ingest\n  method: post\n  operationId: v2-ingest-incident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/gamebooks/rules/{incidentTitle}\n  method: get\n  operationId: v2-get-playbooks-by-incident-title\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/gamebooks/history\n  method: get\n  operationId: v2-list-gamebooks-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/gamebooks/history/{gamebookId}/playbooks\n  method: get\n  operationId: v2-get-playbooks-by-gamebook-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/gamebooks/by-incident/{incidentId}\n  method: get\n  operationId: v2-list-incident-gamebooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/gamebooks/run\n  method: post\n  operationId: v2-run-gamebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/datasources\n\
  \  method: get\n  operationId: v2-get-connected-datasources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/tickets/search\n  method: get\n  operationId: v2-search-tickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/tickets/link\n  method: post\n  operationId: v2-link-ticket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/tickets/unlink\n  method: post\n  operationId: v2-unlink-ticket\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/tickets/priority\n  method: put\n  operationId: v2-update-ticket-priority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/investigation/users/signin-logs\n  method: get\n  operationId: v2-list-signin-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/investigation/users/directory-logs\n  method: get\n  operationId: v2-list-directory-logs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/export/audit\n  method: get\n  operationId: v2-export-audit-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/incidents/{source}/{incidentId}/gamebooks\n  method: post\n  operationId: v2-agent-tool-submit-gamebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/incidents/{source}/{incidentId}/investigation\n  method: post\n  operationId: v2-agent-tool-submit-investigation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/users/{userId}\n  method: get\n  operationId: v2-agent-tool-get-user-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/kql/tables\n  method: get\n  operationId: v2-agent-tool-list-kql-tables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/kql/tables/columns\n  method: post\n  operationId: v2-agent-tool-get-kql-table-columns\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/kql/query\n  method: post\n  operationId: v2-agent-tool-execute-kql\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/users/{userId}/signin-logs\n  method: get\n  operationId: v2-agent-tool-list-signin-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/users/{userId}/directory-logs\n\
  \  method: get\n  operationId: v2-agent-tool-list-directory-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/devices/{deviceId}/timeline\n  method: get\n  operationId: v2-agent-tool-get-device-timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/workspaces/{workspaceId}/agent/tools/incidents/{source}/{incidentId}/related-by-entity\n  method: get\n  operationId: v2-agent-tool-related-incidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/incidents/across-workspaces\n  method: post\n  operationId: v2-list-incidents-across-workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/incidents/across-workspaces/bulk-update\n  method: post\n  operationId: v2-bulk-update-incidents-across-workspaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/gamebooks/across-workspaces/history\n  method: get\n  operationId: v2-list-gamebooks-history-across-workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/datasources/across-workspaces/anomalies\n  method: post\n  operationId: v2-list-datasource-anomalies-across-workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/datasources/across-workspaces\n  method: get\n  operationId: v2-get-datasource-workspaces-across-workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks\n  method: get\n  operationId: v2-list-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks\n  method: post\n  operationId: v2-create-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}\n  method: get\n  operationId: v2-get-webhook\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks/{id}\n  method: put\n  operationId: v2-update-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}\n  method: delete\n  operationId: v2-delete-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/delivery-logs\n  method: get\n  operationId: v2-list-webhook-delivery-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks/{id}/delivery-logs/{logId}\n  method: get\n  operationId: v2-get-webhook-delivery-log\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks/{id}/pause\n  method: post\n  operationId: v2-pause-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/resume\n  method: post\n  operationId: v2-resume-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/enable\n  method: post\n  operationId: v2-enable-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/credentials\n  method: post\n  operationId: v2-update-webhook-credentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/regenerate-secret\n  method: post\n  operationId: v2-regenerate-webhook-secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/test\n  method: post\n  operationId: v2-test-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}/delivery-logs/{logId}/redeliver\n  method: post\n  operationId: v2-redeliver-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/service-accounts\n  method: get\n  operationId: v2-list-service-accounts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/service-accounts\n  method: post\n  operationId: v2-create-service-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/service-accounts/{id}\n  method: get\n  operationId: v2-get-service-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/service-accounts/{id}\n  method: put\n  operationId: v2-update-service-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/service-accounts/{id}\n  method: delete\n  operationId: v2-delete-service-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/service-accounts/{id}/disable\n  method: post\n  operationId: v2-disable-service-account\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/service-accounts/{id}/enable\n  method: post\n  operationId:\
  \ v2-enable-service-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/service-accounts/{id}/credentials\n  method: post\n  operationId: v2-create-service-account-credential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/service-accounts/{id}/credentials/{credentialId}/revoke\n  method: post\n  operationId: v2-revoke-service-account-credential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/service-accounts/sentinel-ingest/deployment-card\n  method: post\n  operationId: v2-provision-sentinel-ingest-credential\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users\n  method: get\n  operationId: v2-list-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users\n  method: post\n  operationId: v2-add-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users\n  method: put\n  operationId: v2-update-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users/{userId}\n  method: get\n  operationId: v2-get-user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/profile\n  method: get\n  operationId: v2-get-user-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/profile\n\
  \  method: put\n  operationId: v2-update-user-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users/workspace/users\n  method: post\n  operationId: v2-get-workspace-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/{id}\n  method: delete\n  operationId: v2-remove-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users/workspace\n  method: post\n  operationId: v2-add-workspace-users\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users/organization/role\n  method: put\n  operationId: v2-update-org-role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/azure-resources/subscriptions\n  method: get\n  operationId: v2-list-azure-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/subscriptions/{subscriptionId}/network-security-groups\n  method: get\n\
  \  operationId: v2-list-azure-nsgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/subscriptions/is-owner\n  method: get\n  operationId: v2-check-azure-subscription-owner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/subscriptions/{subscriptionId}/resource-groups\n  method: get\n  operationId: v2-list-azure-resource-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/subscriptions/{subscriptionId}/resource-groups/{resourceGroup}/workspaces\n  method: get\n  operationId: v2-list-azure-workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/subscriptions/{subscriptionId}/resource-groups/{resourceGroup}/sentinels\n  method: get\n  operationId: v2-list-azure-sentinels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/subscriptions/{subscriptionId}/resource-groups/{resourceGroup}/workspaces/{workspaceName}/validate\n  method: get\n  operationId: v2-validate-azure-workspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/azure-resources/analytical-rules/{ruleId}\n  method: put\n  operationId: v2-update-analytical-rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/agentic-access/contraforce-agentic-access.yml
summary_line: 81 operations · 40 acting · 2 human-in-the-loop
tags:
- Security
- Software-as-a-Service
- Cybersecurity
- Microsoft
- MSP
---
