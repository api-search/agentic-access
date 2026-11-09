---
acting_count: 206
action_class_counts:
  acting: 206
  connected: 134
api_specs:
- filename: bangermail-com-forms-api-openapi.yml
  format: yaml
  label: BangerMail Inc. Forms API
  slug: bangermail-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bangermail-com/openapi/bangermail-com-forms-api-openapi.yml
- filename: bangermail-com-workspaces-api-openapi.yml
  format: yaml
  label: BangerMail Inc. Workspaces API
  slug: bangermail-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bangermail-com/openapi/bangermail-com-workspaces-api-openapi.yml
consequence_counts:
  physical: 35
  read: 134
  safety-critical: 10
  write: 161
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Bangermail Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/workspaces/{workspaceId}/agents/{agentId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/api-keys/{apiKeyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/connections/{connectionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/connections/{connectionId}/grants/{principalKind}/{principalId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/workspaces/{workspaceId}/experiments/{experimentId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/workspaces/{workspaceId}/oauth-clients/{clientId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/products/{productId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspaces/{workspaceId}/provider-connections/{providerConnectionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/workspaces/{workspaceId}/qa/approval-runs/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/ai/email/revise
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/billing/agent-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/billing/spend-limit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/communication-policy/simulate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/drafts/{draftId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/journeys/{journeyId}/render
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/journeys/{journeyKey}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/mailboxes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/mailboxes/sms/numbers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/mailboxes/whatsapp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/workspaces/{workspaceId}/mailboxes/{mailboxId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/{workspaceId}/mailboxes/{mailboxId}/reactivate
operation_count: 340
overview: 'BangerMail Inc. exposes 340 API operations that an AI agent could call, of which 206 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 134 read, 161 write, 35 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BangerMail Inc.
provider_slug: bangermail-com
slug: bangermail-com-agentic-access
source_filename: bangermail-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bangermail-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 340\n  by_action_class:\n    connected: 134\n    acting: 206\n  by_consequence:\n    read: 134\n    physical: 35\n    write: 161\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /v1/workspaces/{workspaceId}/feedback\n  method: get\n  operationId: getCustomerFeedbackAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/feedback\n  method: post\n  operationId: submitCustomerFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/support/messages\n  method: post\n  operationId: sendSupportMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/feedback/attachments\n  method: post\n  operationId: uploadCustomerFeedbackAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/feedback/attachments/prepare\n  method: post\n  operationId: prepareCustomerFeedbackAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/feedback/attachments/{attachmentId}/complete\n  method: post\n  operationId: completeCustomerFeedbackAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/ai/command-runs\n\
  \  method: post\n  operationId: startMailAssistantCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/ai/command-runs/{runId}/tool-results\n  method: post\n  operationId: continueMailAssistantCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/email-preview\n  method: get\n  operationId: getEmailPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}\n  method: patch\n  operationId: renameWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}\n  method: delete\n  operationId:\
  \ deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/select\n  method: post\n  operationId: selectWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/access\n  method: get\n  operationId: getWorkspaceDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/members/{memberId}\n  method: patch\n  operationId: updateWorkspaceMemberRole\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/invitations\n  method: post\n  operationId: createWorkspaceInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/answer-agents\n  method: get\n  operationId: listAnswerAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/answer-agents\n  method: post\n  operationId: createAnswerAgent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/path\n  method: put\n  operationId: selectOnboardingPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/guided\n  method: get\n  operationId: getGuidedOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/onboarding/guided\n  method: post\n  operationId:\
  \ actOnGuidedOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state\n  method: get\n  operationId: getAgentOnboardingState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/start\n  method: post\n  operationId: startAgentOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/aha-one\n\
  \  method: post\n  operationId: ensureAgentOnboardingAhaOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/agent-proof\n  method: post\n  operationId: sendAgentOnboardingProof\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/decision\n  method: put\n  operationId: recordAgentOnboardingDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/domain-choice\n  method: put\n  operationId: chooseAgentOnboardingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/context\n  method: put\n  operationId: submitAgentOnboardingContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/plan\n  method: put\n  operationId: submitAgentOnboardingPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/apply\n  method: post\n  operationId: recordAgentOnboardingImplementation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/plan/approve\n  method: post\n  operationId: approveAgentOnboardingPlan\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/validate\n  method: post\n  operationId: validateAgentOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/agent-state/complete\n  method: post\n  operationId: completeAgentOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/starter-proof\n  method: post\n  operationId: startStarterMailboxProof\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/starter-proof\n  method: get\n  operationId: getStarterMailboxProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/onboarding/domain-proof\n  method: post\n  operationId: startDomainInfrastructureProof\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/domain-proof\n  method: get\n  operationId: getDomainInfrastructureProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/onboarding/goal\n  method: put\n  operationId: selectActivationGoal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/discovery\n  method: get\n  operationId: getWorkspaceDomainDiscovery\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/onboarding/discovery\n  method: post\n  operationId: scanWorkspaceDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/onboarding/discovery\n  method: put\n  operationId: confirmWorkspaceDomainDiscovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/events\n  method: post\n  operationId: sendWorkspaceEvent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks\n  method: get\n  operationId: listProductWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhooks\n  method: post\n  operationId: createProductWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}\n\
  \  method: patch\n  operationId: updateProductWebhookStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}\n  method: delete\n  operationId: deleteProductWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/credentials\n  method: get\n  operationId: getIncomingWebhookCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/deliveries\n  method: get\n  operationId: listProductWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/webhooks/{endpointId}/test\n  method: post\n  operationId: testProductWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/content-settings\n  method: get\n  operationId: getManagedContentSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/content-settings\n\
  \  method: put\n  operationId: putManagedContentSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/communication-policy\n  method: get\n  operationId: getCommunicationPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/communication-policy\n  method: put\n  operationId: putCommunicationPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/communication-policy/simulate\n\
  \  method: post\n  operationId: simulateCommunicationPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/approvals/{approvalId}/managed-layout-preview/{contentId}\n  method: get\n  operationId: getBoundManagedLayoutApprovalPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/approvals/{approvalId}/journey-preview\n  method: get\n  operationId: getJourneyApprovalPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/assets\n\
  \  method: get\n  operationId: listEmailAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/assets\n  method: post\n  operationId: uploadEmailAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/assets/{assetId}\n  method: get\n  operationId: getEmailAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/embed.js\n  method: get\n  operationId: getSignupFormEmbedScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/forms/embed.js\n  method: head\n  operationId: headSignupFormEmbed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/embed.js\n  method: options\n  operationId: optionsembedjsSignupForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/{publicId}/widget\n  method: get\n  operationId: getSignupFormWidget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/{publicId}/widget\n  method: options\n  operationId: optionswidgetSignupForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/{publicId}/subscribe\n\
  \  method: post\n  operationId: submitSignupForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/forms/{publicId}/subscribe\n  method: options\n  operationId: optionssubscribeSignupForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/{publicId}/view\n  method: post\n  operationId: recordSignupFormView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/forms/{publicId}/view\n  method: options\n  operationId:\
  \ optionsviewSignupForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-layouts\n  method: get\n  operationId: listManagedLayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-layouts\n  method: post\n  operationId: createManagedLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-layouts/{layoutId}\n  method: get\n  operationId: getManagedLayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-layouts/{layoutId}\n  method: patch\n  operationId: saveManagedLayoutDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-layouts/{layoutId}/versions\n  method: get\n  operationId: listManagedLayoutVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-layouts/{layoutId}/impact\n  method: get\n  operationId: describeManagedLayoutImpact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /v1/workspaces/{workspaceId}/managed-layouts/{layoutId}/restore\n  method: post\n  operationId: restoreManagedLayoutDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-content\n  method: get\n  operationId: listManagedContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-content\n  method: post\n  operationId: createManagedContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}\n  method: get\n  operationId: getManagedContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}\n  method: patch\n  operationId: updateManagedContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}/render\n  method: post\n  operationId: renderManagedContent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}/translations/{locale}/retry\n  method: post\n  operationId: retryManagedTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}/translations\n  method: get\n  operationId: getManagedContentTranslations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}/translations/{locale}/review\n  method: post\n  operationId:\
  \ reviewManagedContentTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}/versions\n  method: get\n  operationId: listManagedContentPublications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/managed-content/{contentId}/restore\n  method: post\n  operationId: restoreManagedContentRevision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/workspaces/{workspaceId}/journeys\n  method: get\n  operationId: listJourneys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/journeys\n  method: post\n  operationId: createJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}\n  method: delete\n  operationId: deleteJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}\n\
  \  method: get\n  operationId: getJourney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}\n  method: put\n  operationId: updateJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}\n  method: patch\n  operationId: patchJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}/convert-managed\n\
  \  method: post\n  operationId: convertJourneyToManaged\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}/render\n  method: post\n  operationId: renderJourneyManagedEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}/status\n  method: post\n  operationId: setJourneyStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/{workspaceId}/journeys/{journeyId}/preview\n  method: post\n  operationId: previewJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (110 KB total) ---\n# Full source: https://artifacts.apis.io/bangermail-com/agentic-access/bangermail-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/bangermail-com/agentic-access/bangermail-com-agentic-access.yml
summary_line: 340 operations · 206 acting · 10 human-in-the-loop
tags:
- Email Marketing
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Marketing
---
