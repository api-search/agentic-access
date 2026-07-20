---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 64
api_specs:
- filename: accept-midas-openapi-original.yml
  format: yaml
  label: MIDAS API
  slug: midas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accept/refs/heads/main/openapi/accept-midas-openapi-original.yml
consequence_counts:
  read: 64
  safety-critical: 17
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 17
kind: agentic-access
layout: agentic-access
method: generated
name: Accept Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/apply
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/drift_definitions/{id}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/drift_definitions/{id}/deprecate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/drift_definitions/{id}/reject
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/drift_definitions/{id}/retire
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/drift_definitions/{id}/submit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/expectations/{id}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/fail_mode_policies/{id}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/fail_mode_policies/{id}/deprecate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/grants/{id}/reinstate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/grants/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/grants/{id}/suspend
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/plan
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/profiles/{id}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/profiles/{id}/deprecate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/surfaces/{id}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controlplane/surfaces/{id}/deprecate
operation_count: 83
overview: 'Accept exposes 83 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 64 read, 2 write, and 17 safety-critical.


  17 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Accept
provider_slug: accept
slug: accept-agentic-access
source_filename: accept-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/accept-midas-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 83\n  by_action_class:\n    connected: 64\n    acting: 19\n  by_consequence:\n    read: 64\n    write: 2\n    safety-critical: 17\n  human_in_the_loop_required: 17\noperations:\n- path: /healthz\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readyz\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evaluate\n\
  \  method: post\n  operationId: evaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reviews\n  method: post\n  operationId: createReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envelopes\n  method: get\n  operationId: listEnvelopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/envelopes/{id}\n  method: get\n  operationId: getEnvelope\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/escalations\n  method: get\n  operationId: listEscalations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/decisions/request/{requestId}\n  method: get\n  operationId: getDecisionByRequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evidence/envelopes/{id}/audit-events\n  method: get\n  operationId: getEvidenceEnvelopeAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evidence/envelopes/{id}/integrity\n  method: get\n  operationId: getEvidenceEnvelopeIntegrity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evidence/envelopes/{id}/packet\n  method: get\n  operationId: getEvidenceEnvelopePacket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evidence/audit-events\n  method: get\n  operationId: searchEvidenceAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controlplane/apply\n  method: post\n  operationId: applyBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/plan\n  method: post\n  operationId: planBundle\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/audit\n  method: get\n  operationId: listControlAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverage\n  method: get\n  operationId: listGovernanceCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controlplane/surfaces/{id}/approve\n  method: post\n  operationId: approveSurface\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/surfaces/{id}/deprecate\n  method: post\n  operationId: deprecateSurface\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/profiles/{id}/approve\n  method: post\n  operationId: approveProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /v1/controlplane/expectations/{id}/approve\n  method: post\n  operationId: approveGovernanceExpectation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/profiles/{id}/deprecate\n  method: post\n  operationId: deprecateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/fail_mode_policies/{id}/approve\n  method: post\n  operationId: approveFailModePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/fail_mode_policies/{id}/deprecate\n  method: post\n  operationId: deprecateFailModePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/drift_definitions/{id}/submit\n  method: post\n  operationId: submitDriftDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/drift_definitions/{id}/approve\n  method: post\n  operationId: approveDriftDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/drift_definitions/{id}/reject\n  method: post\n  operationId: rejectDriftDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/drift_definitions/{id}/deprecate\n\
  \  method: post\n  operationId: deprecateDriftDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/drift_definitions/{id}/retire\n  method: post\n  operationId: retireDriftDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/grants/{id}/suspend\n  method: post\n  operationId: suspendGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/grants/{id}/revoke\n  method: post\n  operationId: revokeGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controlplane/grants/{id}/reinstate\n  method: post\n  operationId: reinstateGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /v1/surfaces/{id}\n  method: get\n  operationId: getSurface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{id}\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grants\n  method: get\n  operationId: listGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grants/{id}\n  method: get\n  operationId: getGrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/surfaces/{id}/versions\n  method: get\n  operationId: listSurfaceVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/surfaces/{id}/impact\n  method: get\n  operationId: getSurfaceImpact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/surfaces/{id}/recovery\n  method: get\n  operationId: getSurfaceRecovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{id}/versions\n\
  \  method: get\n  operationId: listProfileVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{id}/recovery\n  method: get\n  operationId: getProfileRecovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities\n  method: get\n  operationId: listCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{id}\n  method: get\n  operationId: getCapabilityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{id}/children\n  method: get\n  operationId: listCapabilityChildren\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{id}/businessservices\n  method: get\n  operationId: listCapabilityBusinessServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{id}/ai-bindings\n  method: get\n  operationId: listCapabilityAIBindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/processes\n  method: get\n  operationId: listProcesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/processes/{id}\n  method: get\n  operationId: getProcessById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/processes/{id}/surfaces\n  method: get\n  operationId: listSurfacesByProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businessservices\n  method: get\n  operationId: listBusinessServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businessservices/{id}\n  method: get\n  operationId: getBusinessServiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businessservices/{id}/relationships\n  method: get\n  operationId: listBusinessServiceRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/aisystems\n  method: get\n  operationId: listAISystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aisystems/{id}\n  method: get\n  operationId: getAISystem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aisystems/{id}/versions\n  method: get\n  operationId: listAISystemVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aisystems/{id}/versions/{version}\n  method: get\n  operationId: getAISystemVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aisystems/{id}/bindings\n  method: get\n  operationId: listAISystemBindings\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/graphs/context\n  method: get\n  operationId: getContextGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/graphs/authority\n  method: get\n  operationId: getAuthorityGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/admin-audit\n  method: get\n  operationId: listAdminAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/analytics\n  method: get\n  operationId: getDriftAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/drift/definitions/{id}\n  method: get\n  operationId: getDriftDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/definitions/{id}/versions\n  method: get\n  operationId: listDriftDefinitionVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/definitions/{id}/versions/{version}\n  method: get\n  operationId: getDriftDefinitionVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/definitions/{id}/series\n  method: get\n  operationId: listDriftSeriesByDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/drift/definitions/{id}/observations\n  method: get\n  operationId: listDriftObservationsByDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/series/{id}\n  method: get\n  operationId: getDriftSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/series/{id}/points\n  method: get\n  operationId: listDriftSeriesPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/series/{id}/observations\n  method: get\n  operationId: listDriftObservationsBySeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/series/{id}/annotations\n\
  \  method: get\n  operationId: listDriftAnnotationsBySeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/series-points/{id}\n  method: get\n  operationId: getDriftSeriesPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/observations/{id}\n  method: get\n  operationId: getDriftObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/observations/{id}/annotations\n  method: get\n  operationId: listDriftAnnotationsByObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/annotations/{id}\n  method: get\n  operationId:\
  \ getDriftAnnotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drift/entities/{kind}/{entity_id}/observations\n  method: get\n  operationId: listDriftObservationsByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fail_mode_policies/{id}\n  method: get\n  operationId: getFailModePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fail_mode_policies/{id}/versions\n  method: get\n  operationId: listFailModePolicyVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fail_mode_policies/{id}/versions/{version}\n  method: get\n  operationId:\
  \ getFailModePolicyVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/escalation_targets\n  method: get\n  operationId: listEscalationTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/escalation_targets/{id}\n  method: get\n  operationId: getEscalationTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/escalation_targets/{id}/versions\n  method: get\n  operationId: listEscalationTargetVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/escalation_targets/{id}/versions/{version}\n  method: get\n  operationId: getEscalationTargetVersion\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accept/refs/heads/main/agentic-access/accept-agentic-access.yml
summary_line: 83 operations · 19 acting · 17 human-in-the-loop
tags:
- Company
- Enterprise
- Governance
- AI Agents
- Authority
- Decision Governance
- Audit
- Open Source
---
