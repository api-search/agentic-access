---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 18
api_specs:
- filename: hopae-inc-hconnect-openapi-original.json
  format: json
  label: Hopae hConnect API
  slug: hopae-inc-hconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/openapi/hopae-inc-hconnect-openapi-original.json
consequence_counts:
  read: 18
  safety-critical: 21
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 21
kind: agentic-access
layout: agentic-access
method: generated
name: Hopae Inc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/apps/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/apps/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/production-tests
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/apps/{id}/providers/{providerId}/activation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/providers/{providerId}/activation/documents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/apps/{id}/providers/{providerId}/activation/documents/{documentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/providers/{providerId}/activation/form
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/apps/{id}/redirect-uris
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/rotate-client-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/apps/{id}/webhook-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/webhook-config/rotate-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/workflows
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/apps/{id}/workflows/{workflowId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/apps/{id}/workflows/{workflowId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apps/{id}/workflows/{workflowId}/set-default
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/console/api-keys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/console/api-keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/console/api-keys/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/verifications/dc-request
operation_count: 42
overview: 'Hopae, Inc. exposes 42 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 3 write, and 21 safety-critical.


  21 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hopae, Inc.
provider_slug: hopae-inc
slug: hopae-inc-agentic-access
source_filename: hopae-inc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/hopae-inc-hconnect-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 18\n    acting: 24\n  by_consequence:\n    read: 18\n    write: 3\n    safety-critical: 21\n  human_in_the_loop_required: 21\noperations:\n- path: /v1/providers\n  method: get\n  operationId: getProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verifications/{verificationId}\n  method: get\n  operationId: getVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications/{verificationId}\n  method: delete\n  operationId: deleteVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token\n  method: post\n  operationId: exchangeCodeForToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace\n  method: get\n  operationId: WorkspaceController_getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: post\n  operationId: WorkspaceAppsController_createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps\n  method: get\n  operationId: WorkspaceAppsController_listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/batch\n  method: post\n  operationId:\
  \ WorkspaceAppsController_batchCreateApps\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/redirect-uris\n  method: get\n  operationId: WorkspaceAppsController_getRedirectUris\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/redirect-uris\n  method: put\n  operationId: WorkspaceAppsController_updateRedirectUris\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/apps/{id}/webhook-config\n  method: get\n  operationId: WorkspaceAppsController_getWebhookConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/webhook-config\n  method: patch\n  operationId: WorkspaceAppsController_updateWebhookConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/webhook-config/rotate-secret\n  method: post\n  operationId: WorkspaceAppsController_rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/providers\n  method: get\n  operationId: WorkspaceAppsController_listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}\n  method: get\n  operationId: WorkspaceAppsController_getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}\n  method: patch\n  operationId: WorkspaceAppsController_patchApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/apps/{id}\n  method: delete\n  operationId: WorkspaceAppsController_deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/providers/{providerId}/activation/steps\n  method: get\n  operationId: WorkspaceActivationController_getActivationSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/providers/{providerId}/activation\n  method: patch\n  operationId: WorkspaceActivationController_enableProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/providers/{providerId}/activation/form\n  method: post\n  operationId: WorkspaceActivationController_submitActivationForm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/providers/{providerId}/activation/documents\n  method: post\n  operationId: WorkspaceActivationController_uploadDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/providers/{providerId}/activation/documents/{documentId}\n  method: delete\n  operationId: WorkspaceActivationController_deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/workflows/node-types\n  method: get\n  operationId: WorkspaceWorkflowController_getNodeTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/workflows\n  method: post\n  operationId: WorkspaceWorkflowController_createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/workflows\n  method: get\n  operationId: WorkspaceWorkflowController_listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/workflows/{workflowId}\n  method: get\n  operationId: WorkspaceWorkflowController_getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/workflows/{workflowId}\n  method: patch\n  operationId: WorkspaceWorkflowController_updateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/workflows/{workflowId}\n  method: delete\n  operationId: WorkspaceWorkflowController_deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/workflows/{workflowId}/set-default\n  method: post\n  operationId: WorkspaceWorkflowController_setDefault\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/production-tests\n  method: get\n  operationId: WorkspaceProductionTestController_listChallenges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{id}/production-tests\n  method: post\n  operationId: WorkspaceProductionTestController_createChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/production-tests/{challengeId}/report\n  method: get\n  operationId: WorkspaceProductionTestController_getChallengeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/console/api-keys\n  method: post\n  operationId: ConsoleController_createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/console/api-keys\n  method: get\n  operationId: ConsoleController_listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/console/api-keys/{id}/revoke\n  method: post\n  operationId: ConsoleController_revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/console/api-keys/{id}\n  method: delete\n  operationId: ConsoleController_deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/apps/{id}/rotate-client-secret\n  method: post\n  operationId: WorkspaceAppsController_rotateClientSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/verifications/{verificationId}/evidence\n\
  \  method: get\n  operationId: VerificationController_getVerificationEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications/{verificationId}/userinfo\n  method: get\n  operationId: VerificationController_getVerificationUserinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications/dc-request\n  method: post\n  operationId: VerificationController_createDcRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/providers/{providerId}/configuration\n  method: get\n  operationId:\
  \ ProvidersController_getProviderConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/agentic-access/hopae-inc-agentic-access.yml
summary_line: 42 operations · 24 acting · 21 human-in-the-loop
tags:
- Company
- Identity
- Identity Verification
- Digital Identity
- eID
- Verifiable Credentials
- Authentication
- OpenID Connect
- eIDAS
- KYC
---
