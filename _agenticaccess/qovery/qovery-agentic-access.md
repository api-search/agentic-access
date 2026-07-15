---
acting_count: 271
action_class_counts:
  acting: 271
  connected: 237
api_specs:
- filename: qovery-openapi.yaml
  format: yaml
  label: Qovery
  slug: qovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qovery/main/openapi/qovery-openapi.yaml
consequence_counts:
  physical: 47
  read: 237
  safety-critical: 23
  write: 201
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 23
kind: agentic-access
layout: agentic-access
method: generated
name: Qovery Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /application/{applicationId}/environmentVariable/{environmentVariableId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /application/{applicationId}/restart-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /application/{applicationId}/secret/{secretId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /application/{applicationId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /container/{containerId}/environmentVariable/{environmentVariableId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /container/{containerId}/restart-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /container/{containerId}/secret/{secretId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /container/{containerId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /database/{databaseId}/restart-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /database/{databaseId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environment/{environmentId}/environmentVariable/{environmentVariableId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environment/{environmentId}/secret/{secretId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environment/{environmentId}/service/restart-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environment/{environmentId}/service/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environment/{environmentId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /helm/{helmId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /job/{jobId}/environmentVariable/{environmentVariableId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /job/{jobId}/secret/{secretId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /job/{jobId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{organizationId}/cluster/{clusterId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{projectId}/environmentVariable/{environmentVariableId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{projectId}/secret/{secretId}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /variable/{variableId}/override
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/userSignUp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /application/{applicationId}/deploy
operation_count: 508
overview: 'Qovery exposes 508 API operations that an AI agent could call, of which 271 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 237 read, 201 write, 47 physical, and 23 safety-critical.


  23 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qovery
provider_slug: qovery
slug: qovery-agentic-access
source_filename: qovery-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/qovery-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 508\n  by_action_class:\n    connected: 237\n    acting: 271\n  by_consequence:\n    read: 237\n    write: 201\n    physical: 47\n    safety-critical: 23\n  human_in_the_loop_required: 23\noperations:\n- path: /organization\n  method: get\n  operationId: listOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}\n  method: put\n  operationId: editOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/apiToken\n  method: get\n  operationId: listOrganizationApiTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/apiToken\n  method: post\n  operationId: createOrganizationApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/apiToken/{apiTokenId}\n  method: delete\n  operationId: deleteOrganizationApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/availableRole\n  method: get\n  operationId: listOrganizationAvailableRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/gitToken\n  method: get\n  operationId: listOrganizationGitTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/gitToken\n  method: post\n  operationId: createGitToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /organization/{organizationId}/gitToken/{gitTokenId}\n  method: get\n  operationId: getOrganizationGitToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/gitToken/{gitTokenId}\n  method: put\n  operationId: editGitToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/gitToken/{gitTokenId}\n  method: delete\n  operationId: deleteGitToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/gitToken/{gitTokenId}/associatedServices\n  method: get\n  operationId: getGitTokenAssociatedServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/listDirectoriesFromGitRepository\n  method: post\n  operationId: listDirectoriesFromGitRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/member\n  method: get\n  operationId: getOrganizationMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /organization/{organizationId}/member\n  method: put\n  operationId: editOrganizationMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/member\n  method: delete\n  operationId: deleteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/inviteMember\n  method: get\n  operationId: getOrganizationInvitedMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/inviteMember\n  method: post\n  operationId: postInviteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/inviteMember/{inviteId}\n  method: get\n  operationId: getMemberInvitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/inviteMember/{inviteId}\n  method: post\n  operationId: postAcceptInviteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/inviteMember/{inviteId}\n  method: delete\n  operationId: deleteInviteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/transferOwnership\n  method: post\n  operationId: postOrganizationTransferOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/currentCost\n  method: get\n  operationId:\
  \ getOrganizationCurrentCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/creditCode\n  method: post\n  operationId: addCreditCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/changePlan\n  method: post\n  operationId: changePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/{clusterId}/currentCost\n  method:\
  \ get\n  operationId: getClusterCurrentCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/billingInfo\n  method: get\n  operationId: getOrganizationBillingInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/billingInfo\n  method: put\n  operationId: editOrganizationBillingInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/billingStatus\n  method: get\n  operationId: getOrganizationBillingStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/billingUsageReport\n  method: post\n  operationId: generateBillingUsageReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/billingExternalId\n  method: get\n  operationId: getOrganizationBillingExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/invoice\n  method: get\n  operationId: listOrganizationInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /organization/{organizationId}/invoice/{invoiceId}\n  method: get\n  operationId: getOrganizationInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/invoice/{invoiceId}/download\n  method: get\n  operationId: getOrganizationInvoicePDF\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/downloadInvoices\n  method: post\n  operationId: organizationDownloadAllInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /organization/{organizationId}/creditCard\n  method: get\n  operationId: listOrganizationCreditCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/creditCard\n  method: post\n  operationId: addCreditCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/creditCard/{creditCardId}\n  method: delete\n  operationId: deleteCreditCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /organization/{organizationId}/project\n  method: get\n  operationId: listProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/project\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/project/stats\n  method: get\n  operationId: getOrganizationProjectStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster\n  method: get\n  operationId: listOrganizationCluster\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/status\n  method: get\n  operationId: getOrganizationClusterStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster/{clusterId}\n  method: delete\n  operationId: deleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/{clusterId}\n  method: put\n  operationId: editCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/{clusterId}/status\n  method: get\n  operationId: getClusterStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster/{clusterId}/installationHelmValues\n  method: get\n  operationId: getInstallationHelmValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster/{clusterId}/kubeconfig\n  method: get\n  operationId: getClusterKubeconfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster/{clusterId}/kubeconfig\n  method: put\n  operationId: editClusterKubeconfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/{clusterId}/advancedSettings\n  method: get\n  operationId: getClusterAdvancedSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /organization/{organizationId}/cluster/{clusterId}/advancedSettings\n  method: put\n  operationId: editClusterAdvancedSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/{clusterId}/routingTable\n  method: get\n  operationId: getRoutingTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/cluster/{clusterId}/routingTable\n  method: put\n  operationId: editRoutingTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/cluster/{clusterId}/logs\n  method: get\n  operationId: listClusterLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/aws/credentials\n  method: get\n  operationId: listAWSCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/aws/credentials\n  method: post\n  operationId: createAWSCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/aws/credentials/{credentialsId}\n\
  \  method: get\n  operationId: getAWSCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/aws/credentials/{credentialsId}\n  method: put\n  operationId: editAWSCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/aws/credentials/{credentialsId}\n  method: delete\n  operationId: deleteAWSCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /organization/{organizationId}/onPremise/credentials\n  method: get\n  operationId: listOnPremiseCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/onPremise/credentials\n  method: post\n  operationId: createOnPremiseCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/onPremise/credentials/{credentialsId}\n  method: get\n  operationId: getOnPremiseCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/onPremise/credentials/{credentialsId}\n\
  \  method: put\n  operationId: editOnPremiseCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/onPremise/credentials/{credentialsId}\n  method: delete\n  operationId: deleteOnPremiseCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/scaleway/credentials\n  method: get\n  operationId: listScalewayCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /organization/{organizationId}/scaleway/credentials\n  method: post\n  operationId: createScalewayCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/scaleway/credentials/{credentialsId}\n  method: get\n  operationId: getScalewayCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/scaleway/credentials/{credentialsId}\n  method: put\n  operationId: editScalewayCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/scaleway/credentials/{credentialsId}\n  method: delete\n  operationId: deleteScalewayCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/gcp/credentials\n  method: get\n  operationId: listGcpCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/gcp/credentials\n  method: post\n  operationId: createGcpCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/gcp/credentials/{credentialsId}\n  method: get\n  operationId: getGcpCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/gcp/credentials/{credentialsId}\n  method: put\n  operationId: editGcpCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/gcp/credentials/{credentialsId}\n  method: delete\n  operationId: deleteGcpCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/github/connect\n  method: post\n  operationId: organizationGithubAppConnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/github/disconnect\n  method: delete\n  operationId: organizationGithubAppDisconnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /organization/{organizationId}/account/gitAuthProvider\n  method: get\n  operationId: getOrganizationGitProviderAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/account/github/repository\n  method: get\n  operationId: getOrganizationGithubRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/account/github/repository/branch\n  method: get\n  operationId: getOrganizationGithubRepositoryBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/account/gitlab/repository\n  method: get\n  operationId: getOrganizationGitlabRepositories\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/account/gitlab/repository/branch\n  method: get\n  operationId: getOrganizationGitlabRepositoryBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/account/bitbucket/repository\n  method: get\n  operationId: getOrganizationBitbucketRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/account/bitbucket/repository/branch\n  method: get\n  operationId: getOrganizationBitbucketRepositoryBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/webhook\n\
  \  method: get\n  operationId: listOrganizationWebHooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/webhook\n  method: post\n  operationId: createOrganizationWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/webhook/{webhookId}/event\n  method: get\n  operationId: listWebhookEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/webhook/{webhookId}\n  method: get\n  operationId: getOrganizationWebhook\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/webhook/{webhookId}\n  method: put\n  operationId: editOrganizationWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/webhook/{webhookId}\n  method: delete\n  operationId: deleteOrganizationWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/customRole\n  method: get\n  operationId: listOrganizationCustomRoles\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/customRole\n  method: post\n  operationId: createOrganizationCustomRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/customRole/{customRoleId}\n  method: get\n  operationId: getOrganizationCustomRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/customRole/{customRoleId}\n  method: put\n  operationId: editOrganizationCustomRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/customRole/{customRoleId}\n  method: delete\n  operationId: deleteOrganizationCustomRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/events\n  method: get\n  operationId: getOrganizationEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/targets\n  method: get\n  operationId: getOrganizationEventTargets\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/annotationsGroups\n  method: get\n  operationId: listOrganizationAnnotationsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organizationId}/annotationsGroups\n  method: post\n  operationId: createOrganizationAnnotationsGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organizationId}/annotationsGroups/{annotationsGroupId}\n  method: get\n  operationId: getOrganizationAnnotationsGroup\n  x-agentic-access:\n    action-class: connected\n    conseque\n\n# --- truncated at 32 KB (157 KB total) ---\n\
  # Full source: https://raw.githubusercontent.com/api-evangelist/qovery/refs/heads/main/agentic-access/qovery-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qovery/refs/heads/main/agentic-access/qovery-agentic-access.yml
summary_line: 508 operations · 271 acting · 23 human-in-the-loop
tags:
- Cloud Deployment
- Developer Experience
- Internal Developer Platform
---
