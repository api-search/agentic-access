---
acting_count: 1702
action_class_counts:
  acting: 1702
  connected: 1478
api_specs:
- filename: genesys-platform-api-openapi-original.json
  format: json
  label: Genesys Cloud Platform API
  slug: genesys-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/openapi/genesys-platform-api-openapi-original.json
consequence_counts:
  physical: 90
  read: 1478
  safety-critical: 67
  write: 1545
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 67
kind: agentic-access
layout: agentic-access
method: generated
name: Genesys Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/architect/emergencygroups
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/architect/emergencygroups/{emergencyGroupId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/architect/emergencygroups/{emergencyGroupId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/architect/systemprompts/{promptId}/resources
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/architect/systemprompts/{promptId}/resources/{languageCode}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/architect/systemprompts/{promptId}/resources/{languageCode}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/authorization/policies/targets/{targetName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/authorization/policies/targets/{targetName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/authorization/policies/targets/{targetName}/subject/{subjectId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/authorization/policies/targets/{targetName}/validate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/authorization/policies/{policyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/carrierservices/integrations/emergencylocations/me
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/casemanagement/cases/{caseId}/terminate/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/conversations/calls/{conversationId}/participants/{participantId}/snippet/record
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v2/conversations/emails/{conversationId}/messages/draft
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/conversations/{conversationId}/assign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/conversations/{conversationId}/participants/{participantId}/screenmonitors/sessions/{screenMonitoringId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/diagnostics/logcapture/browser/users/{userId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/emails/settings/threading
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/flows/instances/settings/loglevels/default
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/learning/assignments/{assignmentId}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/outbound/campaigns/{campaignId}/progress
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/outbound/campaigns/{campaignId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/outbound/messagingcampaigns/{messagingCampaignId}/progress
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/outbound/messagingcampaigns/{messagingCampaignId}/stop
operation_count: 3180
overview: 'Genesys exposes 3180 API operations that an AI agent could call, of which 1702 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1478 read, 1545 write, 90 physical, and 67 safety-critical.


  67 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Genesys
provider_slug: genesys
slug: genesys-agentic-access
source_filename: genesys-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/genesys-platform-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3180\n  by_action_class:\n    acting: 1702\n    connected: 1478\n  by_consequence:\n    write: 1545\n    read: 1478\n    safety-critical: 67\n    physical: 90\n  human_in_the_loop_required: 67\noperations:\n- path: /api/v2/events/conversations\n  method: post\n  operationId: postEventsConversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - conversations\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v2/events/users/routingstatus\n  method: post\n  operationId: postEventsUsersRoutingstatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - routing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/events/users/presence\n  method: post\n  operationId: postEventsUsersPresence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - presence\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authorization/divisions/home\n  method: get\n  operationId: getAuthorizationDivisionsHome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisions/limit\n  method: get\n  operationId: getAuthorizationDivisionsLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisions/{divisionId}\n  method: get\n  operationId: getAuthorizationDivision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisions/{divisionId}\n  method: put\n  operationId: putAuthorizationDivision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - authorization\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authorization/divisions/{divisionId}\n  method: delete\n  operationId: deleteAuthorizationDivision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authorization/divisions/{divisionId}/restore\n  method: post\n  operationId: postAuthorizationDivisionRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v2/authorization/divisions/deleted\n  method: get\n  operationId: getAuthorizationDivisionsDeleted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisions/query\n  method: get\n  operationId: getAuthorizationDivisionsQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisions\n  method: get\n  operationId: getAuthorizationDivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisions\n\
  \  method: post\n  operationId: postAuthorizationDivisions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authorization/policies/targets/{targetName}\n  method: get\n  operationId: getAuthorizationPoliciesTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/policies/targets/{targetName}\n  method: post\n  operationId: postAuthorizationPoliciesTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n   \
  \   max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/authorization/policies/targets/{targetName}\n  method: put\n  operationId: putAuthorizationPoliciesTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/authorization/policies/targets/{targetName}/validate\n  method: post\n  operationId: postAuthorizationPoliciesTargetValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - authorization\n    - authorization:readonly\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/authorization/policies\n  method: get\n  operationId: getAuthorizationPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/policies/subject/{subjectId}\n  method: get\n  operationId: getAuthorizationPoliciesSubjectSubjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/policies/targets/{targetName}/subject/{subjectId}\n  method: get\n  operationId: getAuthorizationPoliciesTargetSubjectSubjectId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/policies/targets/{targetName}/subject/{subjectId}\n  method: delete\n  operationId: deleteAuthorizationPoliciesTargetSubjectSubjectId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/authorization/policies/{policyId}\n  method: get\n  operationId: getAuthorizationPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/v2/authorization/policies/{policyId}\n  method: put\n  operationId: putAuthorizationPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - authorization\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/authorization/policies/{policyId}/attributes\n  method: get\n  operationId: getAuthorizationPolicyAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/policies/{policyId}/simulate\n  method: post\n  operationId: postAuthorizationPolicySimulate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - authorization\n    - authorization:readonly\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authorization/policies/targets\n  method: get\n  operationId: getAuthorizationPoliciesTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisionspermitted/me\n  method: get\n  operationId: getAuthorizationDivisionspermittedMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisionspermitted/paged/me\n  method: get\n  operationId: getAuthorizationDivisionspermittedPagedMe\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/divisionspermitted/paged/{subjectId}\n  method: get\n  operationId: getAuthorizationDivisionspermittedPagedSubjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/permissions\n  method: get\n  operationId: getAuthorizationPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authorization/products\n  method: get\n  operationId: getAuthorizationProducts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorization\n    - authorization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/{userId}/verifiers\n  method: get\n  operationId: getUserVerifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - users\n    - users:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/{userId}/verifiers/{verifierId}\n  method: put\n  operationId: putUserVerifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - users\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users/{userId}/verifiers/{verifierId}\n  method: delete\n  operationId: deleteUserVerifier\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - users\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/adfs\n  method: get\n  operationId: getIdentityprovidersAdfs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/adfs\n  method: put\n  operationId: putIdentityprovidersAdfs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/adfs\n\
  \  method: delete\n  operationId: deleteIdentityprovidersAdfs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/cic\n  method: get\n  operationId: getIdentityprovidersCic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/cic\n  method: put\n  operationId: putIdentityprovidersCic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/cic\n  method: delete\n  operationId: deleteIdentityprovidersCic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/gsuite\n  method: get\n  operationId: getIdentityprovidersGsuite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/gsuite\n  method: put\n  operationId: putIdentityprovidersGsuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/gsuite\n  method: delete\n  operationId: deleteIdentityprovidersGsuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/generic\n  method: get\n  operationId: getIdentityprovidersGeneric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/generic\n\
  \  method: put\n  operationId: putIdentityprovidersGeneric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/generic\n  method: delete\n  operationId: deleteIdentityprovidersGeneric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/identitynow\n  method: get\n  operationId: getIdentityprovidersIdentitynow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/identitynow\n  method: put\n  operationId: putIdentityprovidersIdentitynow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/identitynow\n  method: delete\n  operationId: deleteIdentityprovidersIdentitynow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders\n\
  \  method: get\n  operationId: getIdentityproviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders\n  method: post\n  operationId: postIdentityproviders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/{providerId}\n  method: get\n  operationId: getIdentityprovider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/identityproviders/{providerId}\n  method: put\n  operationId: putIdentityprovider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/{providerId}\n  method: delete\n  operationId: deleteIdentityprovider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/oauth/authorizations/{clientId}\n  method: get\n  operationId: getOauthAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - oauth\n    - oauth:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/oauth/authorizations\n  method: get\n  operationId: getOauthAuthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - oauth\n    - oauth:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/oauth/scopes/{scopeId}\n  method: get\n  operationId: getOauthScope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - oauth\n    - oauth:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/oauth/scopes\n  method: get\n  operationId: getOauthScopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - oauth\n    - oauth:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/okta\n  method:\
  \ get\n  operationId: getIdentityprovidersOkta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/okta\n  method: put\n  operationId: putIdentityprovidersOkta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/okta\n  method: delete\n  operationId: deleteIdentityprovidersOkta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/onelogin\n  method: get\n  operationId: getIdentityprovidersOnelogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/onelogin\n  method: put\n  operationId: putIdentityprovidersOnelogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/onelogin\n  method: delete\n  operationId: deleteIdentityprovidersOnelogin\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/ping\n  method: get\n  operationId: getIdentityprovidersPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/ping\n  method: put\n  operationId: putIdentityprovidersPing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/ping\n\
  \  method: delete\n  operationId: deleteIdentityprovidersPing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/purecloud\n  method: get\n  operationId: getIdentityprovidersPurecloud\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/purecloud\n  method: put\n  operationId: putIdentityprovidersPurecloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/purecloud\n  method: delete\n  operationId: deleteIdentityprovidersPurecloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/pureengage\n  method: get\n  operationId: getIdentityprovidersPureengage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/pureengage\n  method: put\n  operationId: putIdentityprovidersPureengage\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/pureengage\n  method: delete\n  operationId: deleteIdentityprovidersPureengage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/salesforce\n  method: get\n  operationId: getIdentityprovidersSalesforce\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity-providers\n    - identity-providers:readonly\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identityproviders/salesforce\n  method: put\n  operationId: putIdentityprovidersSalesforce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identityproviders/salesforce\n  method: delete\n  operationId: deleteIdentityprovidersSalesforce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity-providers\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/organizations/embeddedintegration\n  method: get\n  operationId: getOrganizationsEmbeddedintegration\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - organization\n    - organization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/organizations/embeddedintegration\n  method: put\n  operationId: putOrganizationsEmbeddedintegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - organization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/organizations/ipaddressauthentication\n  method: get\n  operationId: getOrganizationsIpaddressauthentication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - organization\n    - organization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/organizations/ipaddressauthentication\n\
  \  method: put\n  operationId: putOrganizationsIpaddressauthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - organization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/organizations/whitelist\n  method: get\n  operationId: getOrganizationsWhitelist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - organization\n    - organization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/organizations/whitelist\n  method: put\n  operationId: putOrganizationsWhitelist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - organization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/organizations/authentication/settings\n  method: get\n  operationId: getOrganizationsAuthenticationSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - organization\n    - organization:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/organizations/authentication/settings\n  method: patch\n  operationId: patchOrganizationsAuthenticationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - organization\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tokens/me\n  method: get\n  operationId: getTokensMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - user-basic-info\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tokens/me\n  method: head\n  operationId: headTokensMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user-basic-info\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tokens/me\n  method: delete\n  operationId: deleteTokensMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user-basic-info\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tokens/{userId}\n  method: delete\n  operationId: deleteToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user-basic-info\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/users/agentui/agents/autoanswer/{agentId}/settings\n  method: get\n  operationId: getUsersAgentuiAgentsAutoanswerAgentIdSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - users\n    - users:readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/agentui/agents/autoanswer/{agentId}/settings\n  method: put\n  operationId: putUsersAgentuiAgentsAutoanswerAgentIdSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - users\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/u\n\n# --- truncated at 32 KB (1179 KB total) ---\n# Full source:\
  \ https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/agentic-access/genesys-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/agentic-access/genesys-agentic-access.yml
summary_line: 3180 operations · 1702 acting · 67 human-in-the-loop
tags:
- Company
- Software
- Contact Center
- Customer Experience
- CCaaS
- Telephony
- Conversational AI
- Workforce Management
- Cloud Communications
- CPaaS
---
