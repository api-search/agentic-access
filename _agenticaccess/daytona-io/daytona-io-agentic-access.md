---
acting_count: 180
action_class_counts:
  acting: 180
  connected: 150
api_specs:
- filename: daytona-sandbox-api-openapi.yml
  format: yaml
  label: Daytona Sandbox API
  slug: daytona-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-sandbox-api-openapi.yml
- filename: daytona-sandbox-toolbox-api-openapi.yml
  format: yaml
  label: Daytona Sandbox Toolbox API
  slug: daytona-sandbox-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-sandbox-toolbox-api-openapi.yml
- filename: daytona-snapshots-api-openapi.yml
  format: yaml
  label: Daytona Snapshots API
  slug: daytona-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-snapshots-api-openapi.yml
- filename: daytona-volumes-api-openapi.yml
  format: yaml
  label: Daytona Volumes API
  slug: daytona-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-volumes-api-openapi.yml
- filename: daytona-preview-api-openapi.yml
  format: yaml
  label: Daytona Preview API
  slug: daytona-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-preview-api-openapi.yml
- filename: daytona-webhooks-api-openapi.yml
  format: yaml
  label: Daytona Webhooks API
  slug: daytona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-webhooks-api-openapi.yml
- filename: daytona-organizations-api-openapi.yml
  format: yaml
  label: Daytona Organizations API
  slug: daytona-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-organizations-api-openapi.yml
- filename: daytona-api-keys-api-openapi.yml
  format: yaml
  label: Daytona API Keys API
  slug: daytona-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-api-keys-api-openapi.yml
- filename: daytona-users-api-openapi.yml
  format: yaml
  label: Daytona Users API
  slug: daytona-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-users-api-openapi.yml
- filename: daytona-admin-api-openapi.yml
  format: yaml
  label: Daytona Admin API
  slug: daytona-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-admin-api-openapi.yml
- filename: daytona-health-api-openapi.yml
  format: yaml
  label: Daytona Health API
  slug: daytona-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-health-api-openapi.yml
consequence_counts:
  physical: 4
  read: 150
  safety-critical: 12
  write: 164
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Daytona Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /computeruse/recordings/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /computeruse/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lsp/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sandbox/{sandboxIdOrName}/autostop/{interval}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /sandbox/{sandboxIdOrName}/ssh-access
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sandbox/{sandboxIdOrName}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /toolbox/{sandboxId}/toolbox/computeruse/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /toolbox/{sandboxId}/toolbox/lsp/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhooks/organizations/{organizationId}/app-portal-access
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhooks/organizations/{organizationId}/refresh-endpoints
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspace/{workspaceId}/autostop/{interval}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspace/{workspaceId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/webhooks/organizations/{organizationId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /git/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /process/session/{sessionId}/command/{commandId}/input
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /toolbox/{sandboxId}/toolbox/git/checkout
operation_count: 330
overview: 'Daytona exposes 330 API operations that an AI agent could call, of which 180 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 150 read, 164 write, 4 physical, and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Daytona
provider_slug: daytona-io
slug: daytona-io-agentic-access
source_filename: daytona-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/daytona-admin-api-openapi.yml, openapi/daytona-api-keys-api-openapi.yml, openapi/daytona-health-api-openapi.yml,\n  openapi/daytona-organizations-api-openapi.yml, openapi/daytona-preview-api-openapi.yml, openapi/daytona-sandbox-api-openapi.yml,\n  openapi/daytona-sandbox-toolbox-api-openapi.yml, openapi/daytona-snapshots-api-openapi.yml,\n  openapi/daytona-toolbox-api-openapi.yml, openapi/daytona-users-api-openapi.yml, openapi/daytona-volumes-api-openapi.yml,\n  openapi/daytona-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 330\n  by_action_class:\n    connected: 150\n    acting: 180\n  by_consequence:\n    read: 150\n    write: 164\n    physical: 4\n    safety-critical:\
  \ 12\n  human_in_the_loop_required: 12\noperations:\n- path: /config\n  method: get\n  operationId: ConfigController_getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shared-regions\n  method: get\n  operationId: listSharedRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runners\n  method: post\n  operationId: createRunner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runners\n  method: get\n  operationId: listRunners\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runners/me\n  method: get\n  operationId: getInfoForAuthenticatedRunner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runners/by-sandbox/{sandboxId}\n  method: get\n  operationId: getRunnerBySandboxId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runners/by-snapshot-ref\n  method: get\n  operationId: getRunnersBySnapshotRef\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /runners/{id}\n  method: get\n  operationId: getRunnerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runners/{id}\n  method: delete\n  operationId: deleteRunner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runners/{id}/full\n  method: get\n  operationId: getRunnerFullById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runners/{id}/scheduling\n  method:\
  \ patch\n  operationId: updateRunnerScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runners/{id}/draining\n  method: patch\n  operationId: updateRunnerDraining\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runners/healthcheck\n  method: post\n  operationId: runnerHealthcheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    -\
  \ openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/poll\n  method: get\n  operationId: pollJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}/status\n\
  \  method: post\n  operationId: updateJobStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docker-registry\n  method: post\n  operationId: createRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docker-registry\n  method: get\n  operationId: listRegistries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /docker-registry/registry-push-access\n  method: get\n  operationId: getTransientPushAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docker-registry/{id}\n  method: get\n  operationId: getRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docker-registry/{id}\n  method: patch\n  operationId: updateRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /docker-registry/{id}\n  method: delete\n  operationId: deleteRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/runners\n  method: post\n  operationId: adminCreateRunner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/runners\n  method: get\n  operationId: adminListRunners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/runners/{id}\n  method: get\n  operationId: adminGetRunnerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/runners/{id}\n  method: delete\n  operationId: adminDeleteRunner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/runners/{id}/scheduling\n  method: patch\n  operationId: adminUpdateRunnerScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/sandbox/{sandboxId}/recover\n  method: post\n  operationId: adminRecoverSandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users\n  method: post\n  operationId: adminCreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users\n  method: get\n  operationId: adminListUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{id}/regenerate-key-pair\n  method: post\n  operationId: adminRegenerateKeyPair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{id}\n  method: get\n  operationId: adminGetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/webhooks/organizations/{organizationId}/send\n  method: post\n  operationId: adminSendWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/webhooks/organizations/{organizationId}/messages/{messageId}/attempts\n  method: get\n  operationId: adminGetMessageAttempts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/webhooks/status\n  method: get\n  operationId: adminGetWebhookStatus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/webhooks/organizations/{organizationId}/initialize\n  method: post\n  operationId: adminInitializeWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/docker-registry/{id}/set-default\n  method: post\n  operationId: adminSetDefaultRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /admin/snapshots/can-cleanup-image\n  method: get\n  operationId: adminCanCleanupImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/snapshots/{id}/general\n  method: patch\n  operationId: adminSetSnapshotGeneralStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/audit\n  method: get\n  operationId: adminGetAllAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit/organizations/{organizationId}\n  method: get\n  operationId: getOrganizationAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object-storage/push-access\n  method: get\n  operationId: getPushAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/current\n  method: get\n  operationId: getCurrentApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{name}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{name}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys/{userId}/{name}\n  method: delete\n  operationId: deleteApiKeyForUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: HealthController_live\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/ready\n  method: get\n  operationId: HealthController_check\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/invitations\n  method: get\n  operationId: listOrganizationInvitationsForAuthenticatedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/invitations/count\n  method: get\n  operationId: getOrganizationInvitationsCountForAuthenticatedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/invitations/{invitationId}/accept\n  method: post\n  operationId: acceptOrganizationInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/invitations/{invitationId}/decline\n  method: post\n  operationId: declineOrganizationInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/default-region\n  method: patch\n  operationId: setOrganizationDefaultRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/usage\n  method: get\n  operationId: getOrganizationUsageOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/quota\n  method: patch\n  operationId: updateOrganizationQuota\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n\
  \    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/quota/{regionId}\n  method: patch\n  operationId: updateOrganizationRegionQuota\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/leave\n  method: post\n  operationId: leaveOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/suspend\n  method: post\n  operationId: suspendOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/unsuspend\n  method: post\n  operationId: unsuspendOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/otel-config/by-sandbox-auth-token/{authToken}\n\
  \  method: get\n  operationId: getOrganizationOtelConfigBySandboxAuthToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/otel-config\n  method: get\n  operationId: getOrganizationOtelConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/otel-config\n  method: put\n  operationId: updateOrganizationOtelConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /organizations/{organizationId}/otel-config\n  method: delete\n  operationId: deleteOrganizationOtelConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/sandbox-default-limited-network-egress\n  method: post\n  operationId: updateSandboxDefaultLimitedNetworkEgress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/experimental-config\n\
  \  method: put\n  operationId: updateExperimentalConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/roles\n  method: post\n  operationId: createOrganizationRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/roles\n  method: get\n  operationId: listOrganizationRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/roles/{roleId}\n  method: put\n  operationId: updateOrganizationRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/roles/{roleId}\n  method: delete\n  operationId: deleteOrganizationRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /organizations/{organizationId}/users\n  method: get\n  operationId: listOrganizationMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/users/{userId}/access\n  method: post\n  operationId: updateAccessForOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/users/{userId}\n  method: delete\n  operationId: deleteOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n   \
  \ - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/invitations\n  method: post\n  operationId: createOrganizationInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/invitations\n  method: get\n  operationId: listOrganizationInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/invitations/{invitationId}\n\
  \  method: put\n  operationId: updateOrganizationInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/invitations/{invitationId}/cancel\n  method: post\n  operationId: cancelOrganizationInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions\n  method: get\n  operationId: listAvailableRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions\n  method: post\n  operationId: createRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions/{id}\n  method: get\n  operationId: getRegionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/{id}\n  method: delete\n  operationId: deleteRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions/{id}\n  method: patch\n  operationId: updateRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions/{id}/regenerate-proxy-api-key\n  method: post\n  operationId: regenerateProxyApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /regions/{id}/regenerate-ssh-gateway-api-key\n  method: post\n  operationId: regenerateSshGatewayApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions/{id}/regenerate-snapshot-manager-credentials\n  method: post\n  operationId: regenerateSnapshotManagerCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email\n    - openid\n    - profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /preview/{sandboxId}/public\n  method: get\n  operationId: isSandboxPublic\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email\n    - openid\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preview/\n\n# --- truncated at 32 KB (109 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/agentic-access/daytona-io-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/agentic-access/daytona-io-agentic-access.yml
summary_line: 330 operations · 180 acting · 12 human-in-the-loop
tags:
- AI
- Agents
- Artificial Intelligence
- Cloud
- Code Execution
- Computer Use
- Developer Tools
- Infrastructure
- Open Source
- Sandbox
- Secure Execution
---
