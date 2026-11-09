---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 32
api_specs:
- filename: atlas-compiler-com-api-keys-api-openapi.yml
  format: yaml
  label: Atlas API Keys API
  slug: atlas-compiler-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-api-keys-api-openapi.yml
- filename: atlas-compiler-com-billing-api-openapi.yml
  format: yaml
  label: Atlas Billing API
  slug: atlas-compiler-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-billing-api-openapi.yml
- filename: atlas-compiler-com-execution-api-openapi.yml
  format: yaml
  label: Atlas Execution API
  slug: atlas-compiler-com-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-execution-api-openapi.yml
- filename: atlas-compiler-com-identity-api-openapi.yml
  format: yaml
  label: Atlas Identity API
  slug: atlas-compiler-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-identity-api-openapi.yml
- filename: atlas-compiler-com-invitations-api-openapi.yml
  format: yaml
  label: Atlas Invitations API
  slug: atlas-compiler-com-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-invitations-api-openapi.yml
- filename: atlas-compiler-com-jobs-api-openapi.yml
  format: yaml
  label: Atlas Jobs API
  slug: atlas-compiler-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-jobs-api-openapi.yml
- filename: atlas-compiler-com-members-api-openapi.yml
  format: yaml
  label: Atlas Members API
  slug: atlas-compiler-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-members-api-openapi.yml
- filename: atlas-compiler-com-projects-api-openapi.yml
  format: yaml
  label: Atlas Projects API
  slug: atlas-compiler-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-projects-api-openapi.yml
- filename: atlas-compiler-com-system-api-openapi.yml
  format: yaml
  label: Atlas System API
  slug: atlas-compiler-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-system-api-openapi.yml
- filename: atlas-compiler-com-usage-api-openapi.yml
  format: yaml
  label: Atlas Usage API
  slug: atlas-compiler-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-usage-api-openapi.yml
- filename: atlas-compiler-com-webhooks-api-openapi.yml
  format: yaml
  label: Atlas Webhooks API
  slug: atlas-compiler-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-webhooks-api-openapi.yml
- filename: atlas-compiler-com-workspaces-api-openapi.yml
  format: yaml
  label: Atlas Workspaces API
  slug: atlas-compiler-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlas-compiler-com/openapi/atlas-compiler-com-workspaces-api-openapi.yml
consequence_counts:
  physical: 5
  read: 32
  safety-critical: 2
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Atlas Compiler Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/api-keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/invitations/{invitationId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/billing/checkout/reconcile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/billing/topup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/members/{userId}/transfer-ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/test
operation_count: 70
overview: 'Atlas exposes 70 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 31 write, 5 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atlas
provider_slug: atlas-compiler-com
slug: atlas-compiler-com-agentic-access
source_filename: atlas-compiler-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/atlas-compiler-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 70\n  by_action_class:\n    connected: 32\n    acting: 38\n  by_consequence:\n    read: 32\n    write: 31\n    safety-critical: 2\n    physical: 5\n  human_in_the_loop_required: 2\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bootstrap\n  method: get\n  operationId: getWorkspaceBootstrap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/compile\n  method: post\n  operationId: compileUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crawls\n  method: post\n  operationId: createCrawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/invitations/accept\n  method: post\n  operationId: acceptInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/cancel\n  method: post\n  operationId: bulkCancelJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}\n  method: delete\n  operationId:\
  \ cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{jobId}/errors\n  method: get\n  operationId: listJobErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{jobId}/results\n  method: get\n  operationId: listJobResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/map\n  method: post\n  operationId: mapUrl\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape\n  method: post\n  operationId: scrapeUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/by-slug/{workspaceSlug}\n  method: get\n  operationId: resolveWorkspaceBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}\n  method: patch\n  operationId: updateWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/api-keys/{keyId}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workspaces/{workspaceId}/api-keys/{keyId}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/api-keys/{keyId}/regenerate\n  method: post\n  operationId: regenerateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/api-keys/{keyId}/roll\n  method: post\n  operationId: rollApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/api-keys/{keyId}/rotate\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/billing/checkout\n  method: post\n  operationId: createBillingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/billing/checkout/reconcile\n  method: post\n  operationId: reconcileBillingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/billing/invoices\n  method: get\n  operationId: getBillingInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/billing/portal\n  method: post\n  operationId: createBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/billing/preview\n  method: post\n  operationId: previewBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/billing/subscription\n  method: get\n  operationId: getBillingSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/billing/topup\n  method: post\n  operationId: createBillingTopupCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/billing/topups\n  method: get\n  operationId: getBillingTopupCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/deletion\n  method: get\n  operationId: getWorkspaceDeletion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/invitations\n  method: get\n  operationId: listWorkspaceInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/invitations\n  method: post\n  operationId: createWorkspaceInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/invitations/accept\n  method: post\n\
  \  operationId: acceptWorkspaceInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/invitations/{invitationId}\n  method: delete\n  operationId: revokeWorkspaceInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workspaces/{workspaceId}/leave\n  method: delete\n  operationId: leaveWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/members\n  method: get\n  operationId: listWorkspaceMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/members/{userId}\n  method: delete\n  operationId: removeWorkspaceMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/members/{userId}\n  method: patch\n  operationId: updateWorkspaceMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/members/{userId}/transfer-ownership\n  method: post\n  operationId: transferWorkspaceOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/overview\n  method: get\n  operationId: getWorkspaceOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - usage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/projects-stats\n  method: get\n  operationId: getProjectsStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/projects/{projectId}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/usage/ledger\n\
  \  method: get\n  operationId: listUsageLedger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhook-deliveries\n  method: get\n  operationId: listWorkspaceWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhook-deliveries/{deliveryId}\n  method: get\n  operationId: getWorkspaceWebhookDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhook-deliveries/{deliveryId}/attempts\n  method: get\n  operationId: listWorkspaceWebhookDeliveryAttempts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhook-deliveries/{deliveryId}/redeliver\n  method: post\n  operationId: redeliverWorkspaceWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhook-secret\n  method: get\n  operationId: getWorkspaceWebhookSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhook-secret/rotate\n  method: post\n  operationId: rotateWorkspaceWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhooks\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/deliveries/{deliveryId}/redeliver\n  method: post\n  operationId: redeliverWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/test\n  method: post\n  operationId: sendWebhookTestEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/atlas-compiler-com/agentic-access/atlas-compiler-com-agentic-access.yml
summary_line: 70 operations · 38 acting · 2 human-in-the-loop
tags:
- Web Intelligence
- Data Pipeline
- Automation
- Artificial Intelligence
- Developer Tools
---
