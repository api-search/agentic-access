---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 42
api_specs:
- filename: yuzu-health-openapi-original.json
  format: json
  label: Yuzu API
  slug: yuzu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-openapi-original.json
consequence_counts:
  read: 42
  safety-critical: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 34
kind: agentic-access
layout: agentic-access
method: generated
name: Yuzu Health Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/claims/medical/institutional/{coverageId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/claims/medical/professional/{coverageId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/claims/pharmacy/{coverageId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/claims/plan/{planId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/coverages/{coverageId}/fees
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/coverages/{coverageId}/fees/{coverageFeeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/coverages/{coverageId}/fees/{coverageFeeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/networks/{networkId}/providers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/planFees/{planFeeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/plans/{planId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/plans/{planId}/benefits
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/providers/{networkProviderId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/providers/{networkProviderId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sponsors
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/sponsors/{sponsorNamespace}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sponsors/{sponsorNamespace}/enroll/initial-enrollment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/coverages/{coverageId}/benefit-lookup/codes/{code}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/coverages/{coverageId}/care-events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/coverages/{coverageId}/care-events/{careEventId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/coverages/{coverageId}/care-events/{careEventId}/replacement
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/enroll/{enrollmentRequestId}/status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/groups
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/groups/{groupPolicyId}/enroll/initial-enrollment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/groups/{groupPolicyId}/enroll/new-subscribers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/groups/{groupPolicyId}/plans/add
operation_count: 76
overview: 'Yuzu Health exposes 76 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 42 read and 34 safety-critical.


  34 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yuzu Health
provider_slug: yuzu-health
slug: yuzu-health-agentic-access
source_filename: yuzu-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/yuzu-health-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    connected: 42\n    acting: 34\n  by_consequence:\n    read: 42\n    safety-critical: 34\n  human_in_the_loop_required: 34\noperations:\n- path: /v1/members\n  method: get\n  operationId: PublicApiV1Controller_listAllMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/members/{memberId}\n  method: get\n  operationId: PublicApiV1Controller_getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/networks\n  method: get\n  operationId: PublicApiV1Controller_listAllNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/networks/{networkId}/providers\n  method: get\n  operationId: PublicApiV1Controller_listAllProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/networks/{networkId}/providers\n  method: post\n  operationId: PublicApiV1Controller_createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/providers/{networkProviderId}\n  method:\
  \ patch\n  operationId: PublicApiV1Controller_updateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/providers/{networkProviderId}\n  method: delete\n  operationId: PublicApiV1Controller_deleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/coverages/{coverageId}\n  method: get\n  operationId: PublicApiV1Controller_getCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverages/{coverageId}/fees\n  method: post\n  operationId: PublicApiV1Controller_createCoverageFee\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/coverages/{coverageId}/fees/{coverageFeeId}\n  method: patch\n  operationId: PublicApiV1Controller_updateCoverageFee\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/coverages/{coverageId}/fees/{coverageFeeId}\n  method: delete\n  operationId:\
  \ PublicApiV1Controller_deleteCoverageFee\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sponsors\n  method: post\n  operationId: PublicApiV1Controller_createSponsor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sponsors\n  method: get\n  operationId: PublicApiV1Controller_listAllSponsors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/sponsors/{sponsorNamespace}\n  method: get\n  operationId: PublicApiV1Controller_getSponsor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sponsors/{sponsorNamespace}\n  method: patch\n  operationId: PublicApiV1Controller_updateSponsor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sponsors/{sponsorNamespace}/enroll/initial-enrollment\n  method: post\n  operationId: PublicApiV1Controller_createInitialEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n \
  \     purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sponsors/{sponsorNamespace}/members\n  method: get\n  operationId: PublicApiV1Controller_listSponsorMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans/{planId}/vendorRelationships\n  method: get\n  operationId: PublicApiV1Controller_listVendorRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans/{planId}\n  method: delete\n  operationId: PublicApiV1Controller_deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/planFees/{planFeeId}\n  method: post\n  operationId: PublicApiV1Controller_editPlanFee\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/vendors/{vendorId}\n  method: get\n  operationId: PublicApiV1Controller_getVendor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vendors\n  method: get\n  operationId: PublicApiV1Controller_listAllVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/medical/{claimId}\n\
  \  method: get\n  operationId: PublicApiV1Controller_getMedicalClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/medical\n  method: get\n  operationId: PublicApiV1Controller_listAllMedicalClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/pharmacy/{claimId}\n  method: get\n  operationId: PublicApiV1Controller_getPharmacyClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/pharmacy\n  method: get\n  operationId: PublicApiV1Controller_listAllPharmacyClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/preCerts/{preCertId}\n\
  \  method: get\n  operationId: PublicApiV1Controller_getPreCert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/preCerts\n  method: get\n  operationId: PublicApiV1Controller_listAllPreCerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cashCards/{cashCardId}\n  method: get\n  operationId: PublicApiV1Controller_getCashCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrollmentRequests/{enrollmentRequestId}\n  method: get\n  operationId: PublicApiV1Controller_getEnrollmentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/submittedAccumulatorRollovers/{submittedAccumulatorRolloverId}\n\
  \  method: get\n  operationId: PublicApiV1Controller_getSubmittedAccumulatorRollover\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/plan/{planClaimId}\n  method: get\n  operationId: PublicApiV1Controller_getPlanClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/plan\n  method: get\n  operationId: PublicApiV1Controller_getPaginatedPlanClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/plan/{planId}\n  method: post\n  operationId: PublicApiV1Controller_createPlanClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/claims/pharmacy/{coverageId}\n  method: post\n  operationId: PublicApiV1Controller_createPharmacyClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/claims/medical/professional/{coverageId}\n  method: post\n  operationId: PublicApiV1Controller_createProfessionalClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/claims/medical/institutional/{coverageId}\n  method: post\n  operationId: PublicApiV1Controller_createInstitutionalClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/plans/{planId}/benefits\n  method: get\n  operationId: PublicApiV1Controller_getBenefits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans/{planId}/benefits\n  method: patch\n  operationId: PublicApiV1Controller_setBenefits\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/plans/{planId}/sbc\n  method: get\n  operationId: PublicApiV1Controller_getSbc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups\n  method: post\n  operationId: PublicApiV2Controller_createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/groups\n  method: get\n  operationId: PublicApiV2Controller_listAllGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/groups/{groupPolicyId}\n  method: get\n  operationId: PublicApiV2Controller_getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups/{groupPolicyId}/enroll/initial-enrollment\n  method: post\n  operationId: PublicApiV2Controller_createInitialEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/groups/{groupPolicyId}/enroll/new-subscribers\n  method: post\n  operationId: PublicApiV2Controller_createNewSubscribersEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/enroll/{enrollmentRequestId}/status\n  method: post\n  operationId: PublicApiV2Controller_getEnrollmentRequestStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/groups/{groupPolicyId}/members\n  method: get\n  operationId: PublicApiV2Controller_listGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups/{groupPolicyId}/plans/remove/{planIdToRemove}\n  method: delete\n  operationId: PublicApiV2Controller_removePlanFromGroup\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/groups/{groupPolicyId}/plans/add\n  method: post\n  operationId: PublicApiV2Controller_addPlanToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/plans/{planId}/spd\n  method: get\n  operationId: PublicApiV2Controller_getSpd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/designs\n\
  \  method: get\n  operationId: PublicApiV2Controller_getDesigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/care-events\n  method: post\n  operationId: PublicApiV2Controller_createCareEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/coverages/{coverageId}/care-events\n  method: get\n  operationId: PublicApiV2Controller_listCareEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/care-events/{careEventId}/replacement\n  method: post\n  operationId:\
  \ PublicApiV2Controller_replaceCareEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/coverages/{coverageId}/care-events/{careEventId}\n  method: delete\n  operationId: PublicApiV2Controller_deleteCareEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/designs/{planDesignId}/benefits\n  method: get\n  operationId: PublicApiV2Controller_getDesignBenefits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accumulator/coverage/buckets/{coverageId}\n  method: get\n  operationId: PublicAccumulatorController_getCoverageBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accumulator/coverage/{coverageId}\n  method: get\n  operationId: PublicAccumulatorController_getCoverageAccums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/benefit-lookup\n  method: get\n  operationId: PublicBenefitsController_getBenefitLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/benefit-lookup/codes/{code}\n  method: post\n  operationId: PublicBenefitsController_getBenefitLookupByCode\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/eob/download/{claimId}\n  method: get\n  operationId: PublicEobController_downloadEob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/generate-id-card/svg\n  method: get\n  operationId: PublicCoverageController_generateIDCardSvg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/generate-id-card/b64\n  method: get\n  operationId: PublicCoverageController_generateIDCardB64\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverages/{coverageId}/generate-id-card/pdf\n  method: get\n  operationId: PublicCoverageController_generateIDCardPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/groups/{groupPolicyId}/enroll/add-subscriber\n  method: post\n  operationId: PublicEnrollmentApplicationController_createAddSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/groups/{groupPolicyId}/enroll/{subscriberCoverageId}/add-dependent\n  method: post\n  operationId: PublicEnrollmentApplicationController_createAddDependent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/groups/{groupPolicyId}/enroll/terminate\n  method: post\n  operationId: PublicEnrollmentApplicationController_createTermination\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/groups/{groupPolicyId}/renew\n  method: post\n  operationId: PublicGroupPolicyController_renewGroupPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/groups/{groupPolicyId}/rules\n  method: get\n  operationId: PublicGroupPolicyController_getGroupPolicyRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/groups/{groupPolicyId}/rules\n  method: patch\n  operationId: PublicGroupPolicyController_updateGroupPolicyRules\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/members\n  method: get\n  operationId: PublicMemberController_listAllMembers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{memberId}\n  method: get\n  operationId: PublicMemberController_getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{memberId}\n  method: patch\n  operationId: PublicMemberController_updateMemberDemographics\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/members/{memberId}/updateLogin\n  method: post\n  operationId: PublicMemberController_updateMemberLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/sponsors/{sponsorNamespace}\n  method: get\n  operationId: SponsorPublicController_getSponsor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sponsors/{sponsorNamespace}\n  method: patch\n  operationId: SponsorPublicController_updateSponsor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/agentic-access/yuzu-health-agentic-access.yml
summary_line: 76 operations · 34 acting · 34 human-in-the-loop
tags:
- Company
- Health
- Healthcare
- Insurance
- Health Plans
- Benefits Administration
- Claims
- Enrollment
- Payers
- Self-Funded
---
