---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 53
api_specs:
- filename: obol-openapi-original.json
  format: json
  label: Obol API
  slug: obol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-openapi-original.json
- filename: docs-json
  format: yaml
  label: Obol API OpenAPI (live)
  slug: obol-api-openapi-live
  spec_type: OpenAPI
  url: https://api.obol.tech/docs-json
consequence_counts:
  read: 53
  safety-critical: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Obol Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /deposit_data/partial_deposits/{lockHash}/{share_index}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /exp/partial_exits/{lockHash}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fee_recipient/partial/{lockHash}/{shareIdx}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fee_recipient/{lockHash}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lock
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lock/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /positions/{network}/{address}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/definition
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/definition/{configHash}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/deposit_data/partial_deposits/{lockHash}/{share_index}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/exp/partial_exits/{lockHash}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/fee_recipient/partial/{lockHash}/{shareIdx}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/fee_recipient/{lockHash}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/lock
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/lock/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/positions/{network}/{address}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/termsAndConditions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/test
operation_count: 71
overview: 'Obol exposes 71 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 53 read and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Obol
provider_slug: obol
slug: obol-agentic-access
source_filename: obol-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/obol-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    connected: 53\n    acting: 18\n  by_consequence:\n    read: 53\n    safety-critical: 18\n  human_in_the_loop_required: 18\noperations:\n- path: /\n  method: get\n  operationId: AppController_redirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/_health\n  method: get\n  operationId: HealthController_check_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n\
  \  method: get\n  operationId: MetricsController_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/definition/{configHash}\n  method: get\n  operationId: DefinitionController_getClusterDefinition_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/definition/{configHash}\n  method: put\n  operationId: DefinitionController_updateClusterDefinition_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/definition/operator\n  method: get\n  operationId: DefinitionController_getClusterDefinitionWithOperator[0]_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/definition/operator/{address}\n  method: get\n  operationId: DefinitionController_getClusterDefinitionWithOperator[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/definition\n  method: post\n  operationId: DefinitionController_postClusterDefinition_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /lock/{lockHash}\n  method: get\n  operationId: LockController_getClusterLock[0]\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/{lockHash}\n  method: get\n  operationId: LockController_getClusterLock[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/search/{network}\n  method: get\n  operationId: LockController_searchClusterLocks[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/search/{network}\n  method: get\n  operationId: LockController_searchClusterLocks[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/configHash/{configHash}\n  method: get\n  operationId: LockController_getLockByConfigHash[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/configHash/{configHash}\n  method: get\n  operationId: LockController_getLockByConfigHash[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/{lockHash}/launchpad\n  method: get\n  operationId: LockController_redirectToClusterStatus[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/{lockHash}/launchpad\n  method: get\n  operationId: LockController_redirectToClusterStatus[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/{lockHash}/peer-scores\n  method: get\n  operationId: LockController_getAveragePeerScores[0]\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/{lockHash}/peer-scores\n  method: get\n  operationId: LockController_getAveragePeerScores[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/operator\n  method: get\n  operationId: LockController_getClusterLocksByOperator[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/operator/{address}\n  method: get\n  operationId: LockController_getClusterLocksByOperator[1]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/operator\n  method: get\n  operationId: LockController_getClusterLocksByOperator[2]_v1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/operator/{address}\n  method: get\n  operationId: LockController_getClusterLocksByOperator[3]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/network/{network}\n  method: get\n  operationId: LockController_getClusterLocksByNetwork[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/network/{network}\n  method: get\n  operationId: LockController_getClusterLocksByNetwork[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock/network/summary/{network}\n  method: get\n  operationId: LockController_getClusterLockNetworkSummary[0]\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lock/network/summary/{network}\n  method: get\n  operationId: LockController_getClusterLockNetworkSummary[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lock\n  method: post\n  operationId: LockController_postClusterLock[0]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/lock\n  method: post\n  operationId: LockController_postClusterLock[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /lock/verify\n  method: post\n  operationId: LockController_verifyClusterLock[0]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/lock/verify\n  method: post\n  operationId: LockController_verifyClusterLock[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/state/{lockHash}\n  method: get\n  operationId: StateController_getDistributedValidatorStatesByLockHash_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exp/exit/status/summary/{lockHash}\n  method: get\n  operationId: ExitController_getClusterExitStatusSummary[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exp/exit/status/summary/{lockHash}\n  method: get\n  operationId: ExitController_getClusterExitStatusSummary[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exp/exit/status/{lockHash}\n  method: get\n  operationId: ExitController_getClusterExitStatus[0]\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exp/exit/status/{lockHash}\n  method: get\n  operationId: ExitController_getClusterExitStatus[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exp/exit/{lockHash}/{shareIdx}/{validatorPubkey}\n  method: get\n  operationId: ExitController_getClusterExit[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exp/exit/{lockHash}/{shareIdx}/{validatorPubkey}\n  method: get\n  operationId: ExitController_getClusterExit[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exp/partial_exits/{lockHash}\n  method: post\n  operationId: ExitController_postPartialExit[0]\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/exp/partial_exits/{lockHash}\n  method: post\n  operationId: ExitController_postPartialExit[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/effectiveness/{lockHash}\n  method: get\n  operationId: EffectivenessController_getClusterLock_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/termsAndConditions\n\
  \  method: post\n  operationId: TermsAndConditionsController_signTermsAndConditions_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/termsAndConditions/{address}\n  method: get\n  operationId: TermsAndConditionsController_getTermsAndConditionsSigned_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/techne/base/{index}\n  method: get\n  operationId: TechneController_getBaseCred_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/techne/bronze/{index}\n  method: get\n  operationId: TechneController_getBronzeCred_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/techne/silver/{index}\n  method: get\n  operationId: TechneController_getSilverCred_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/techne/gold/{index}\n  method: get\n  operationId: TechneController_getGoldCred_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/techne/{address}\n  method: get\n  operationId: AddressController_getAddressTechneCredentials_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/badges/{address}\n  method: get\n  operationId: AddressController_getAddressBadgess_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/incentives/{network}/{address}\n  method: get\n  operationId: AddressController_getAddressIncentives_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/incentives/historical/{network}/{address}\n  method: get\n  operationId: AddressController_getHistoricalAddressContributions_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/network/{network}\n  method: get\n  operationId: AddressController_getOperatorsByNetwork_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/search/{network}\n\
  \  method: get\n  operationId: AddressController_searchOperators_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/migrateable-validators/{network}/{withdrawalAddress}\n  method: get\n  operationId: AddressController_getMigrateableValidators_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owr/{network}/{address}\n  method: get\n  operationId: OWRController_get_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/migrate/{network}\n  method: get\n  operationId: MigrateController_getValidatorsMigrateStatus_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/test\n  method: post\n  operationId: TestController_postTestResult_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/test/enr/{enr}\n  method: get\n  operationId: TestController_getTestResultByEnr_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit_data/{lockHash}/{pubkey}\n  method: get\n  operationId: DepositController_getDeposits[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deposit_data/{lockHash}/{pubkey}\n  method: get\n  operationId: DepositController_getDeposits[1]_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit_data/partial_deposits/{lockHash}/{share_index}\n  method: post\n  operationId: DepositController_submitPartialDeposits[0]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/deposit_data/partial_deposits/{lockHash}/{share_index}\n  method: post\n  operationId: DepositController_submitPartialDeposits[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /fee_recipient/partial/{lockHash}/{shareIdx}\n  method: post\n  operationId: FeeRecipientController_postPartialFeeRecipients[0]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/fee_recipient/partial/{lockHash}/{shareIdx}\n  method: post\n  operationId: FeeRecipientController_postPartialFeeRecipients[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fee_recipient/{lockHash}\n\
  \  method: post\n  operationId: FeeRecipientController_getPartialFeeRecipients[0]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/fee_recipient/{lockHash}\n  method: post\n  operationId: FeeRecipientController_getPartialFeeRecipients[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tvs/{network}\n  method: get\n  operationId: TVSController_getTVS[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tvs/{network}\n  method: get\n  operationId: TVSController_getTVS[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/{network}/{address}\n  method: post\n  operationId: PositionsController_getPositions[0]\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/positions/{network}/{address}\n  method: post\n  operationId: PositionsController_getPositions[1]_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n   \
  \   purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eth-apr\n  method: get\n  operationId: EthAprController_getEthApr[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eth-apr\n  method: get\n  operationId: EthAprController_getEthApr[1]_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/agentic-access/obol-agentic-access.yml
summary_line: 71 operations · 18 acting · 18 human-in-the-loop
tags:
- Company
- Crypto
- Ethereum
- Staking
- Distributed Validators
- Blockchain Infrastructure
- Web3
---
