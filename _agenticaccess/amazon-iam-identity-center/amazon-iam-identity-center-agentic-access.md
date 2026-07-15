---
acting_count: 56
action_class_counts:
  acting: 56
api_specs:
- filename: amazon-iam-identity-center-sso-admin-openapi-original.yml
  format: yaml
  label: AWS IAM Identity Center SSO Admin API
  slug: aws-sso-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/openapi/amazon-iam-identity-center-sso-admin-openapi-original.yml
- filename: amazon-iam-identity-center-identitystore-openapi-original.yml
  format: yaml
  label: AWS IAM Identity Center Identity Store API
  slug: aws-identitystore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/openapi/amazon-iam-identity-center-identitystore-openapi-original.yml
consequence_counts:
  physical: 11
  safety-critical: 4
  write: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Iam Identity Center Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=SWBExternalService.CreateInstanceAccessControlAttributeConfiguration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=SWBExternalService.DeleteInstanceAccessControlAttributeConfiguration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=SWBExternalService.DescribeInstanceAccessControlAttributeConfiguration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=SWBExternalService.UpdateInstanceAccessControlAttributeConfiguration
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIdentityStore.CreateGroupMembership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIdentityStore.DeleteGroupMembership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIdentityStore.DescribeGroupMembership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIdentityStore.GetGroupMembershipId
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIdentityStore.ListGroupMemberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIdentityStore.ListGroupMembershipsForMember
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=SWBExternalService.DescribePermissionSetProvisioningStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=SWBExternalService.ListAccountsForProvisionedPermissionSet
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=SWBExternalService.ListPermissionSetProvisioningStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=SWBExternalService.ListPermissionSetsProvisionedToAccount
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=SWBExternalService.ProvisionPermissionSet
operation_count: 56
overview: 'Amazon IAM Identity Center exposes 56 API operations that an AI agent could call, of which 56 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 write, 11 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
slug: amazon-iam-identity-center-agentic-access
source_filename: amazon-iam-identity-center-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-iam-identity-center-identitystore-openapi-original.yml, openapi/amazon-iam-identity-center-sso-admin-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    acting: 56\n  by_consequence:\n    write: 41\n    physical: 11\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /#X-Amz-Target=AWSIdentityStore.CreateGroup\n  method: post\n  operationId: CreateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.CreateGroupMembership\n  method: post\n  operationId: CreateGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.CreateUser\n  method: post\n  operationId: CreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.DeleteGroup\n  method: post\n  operationId: DeleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.DeleteGroupMembership\n  method: post\n  operationId: DeleteGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.DeleteUser\n  method: post\n  operationId: DeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.DescribeGroup\n  method: post\n  operationId: DescribeGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.DescribeGroupMembership\n  method: post\n  operationId: DescribeGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.DescribeUser\n  method: post\n  operationId: DescribeUser\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.GetGroupId\n  method: post\n  operationId: GetGroupId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.GetGroupMembershipId\n  method: post\n  operationId: GetGroupMembershipId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.GetUserId\n  method: post\n  operationId: GetUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.IsMemberInGroups\n  method: post\n  operationId: IsMemberInGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.ListGroupMemberships\n  method: post\n  operationId: ListGroupMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.ListGroupMembershipsForMember\n  method: post\n  operationId: ListGroupMembershipsForMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.ListGroups\n  method: post\n  operationId: ListGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.ListUsers\n  method: post\n  operationId: ListUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.UpdateGroup\n  method: post\n  operationId: UpdateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIdentityStore.UpdateUser\n  method: post\n  operationId: UpdateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.AttachCustomerManagedPolicyReferenceToPermissionSet\n  method: post\n  operationId: AttachCustomerManagedPolicyReferenceToPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.AttachManagedPolicyToPermissionSet\n  method: post\n  operationId: AttachManagedPolicyToPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.CreateAccountAssignment\n  method: post\n  operationId: CreateAccountAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.CreateInstanceAccessControlAttributeConfiguration\n  method: post\n  operationId: CreateInstanceAccessControlAttributeConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.CreatePermissionSet\n\
  \  method: post\n  operationId: CreatePermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DeleteAccountAssignment\n  method: post\n  operationId: DeleteAccountAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DeleteInlinePolicyFromPermissionSet\n  method: post\n  operationId: DeleteInlinePolicyFromPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DeleteInstanceAccessControlAttributeConfiguration\n  method: post\n  operationId: DeleteInstanceAccessControlAttributeConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DeletePermissionSet\n  method: post\n  operationId: DeletePermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DeletePermissionsBoundaryFromPermissionSet\n  method: post\n  operationId: DeletePermissionsBoundaryFromPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DescribeAccountAssignmentCreationStatus\n  method: post\n  operationId: DescribeAccountAssignmentCreationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DescribeAccountAssignmentDeletionStatus\n  method: post\n\
  \  operationId: DescribeAccountAssignmentDeletionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DescribeInstanceAccessControlAttributeConfiguration\n  method: post\n  operationId: DescribeInstanceAccessControlAttributeConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DescribePermissionSet\n  method: post\n  operationId: DescribePermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DescribePermissionSetProvisioningStatus\n  method: post\n  operationId: DescribePermissionSetProvisioningStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DetachCustomerManagedPolicyReferenceFromPermissionSet\n  method: post\n  operationId: DetachCustomerManagedPolicyReferenceFromPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.DetachManagedPolicyFromPermissionSet\n  method: post\n  operationId: DetachManagedPolicyFromPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.GetInlinePolicyForPermissionSet\n  method: post\n  operationId: GetInlinePolicyForPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /#X-Amz-Target=SWBExternalService.GetPermissionsBoundaryForPermissionSet\n  method: post\n  operationId: GetPermissionsBoundaryForPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListAccountAssignmentCreationStatus\n  method: post\n  operationId: ListAccountAssignmentCreationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListAccountAssignmentDeletionStatus\n  method: post\n  operationId: ListAccountAssignmentDeletionStatus\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListAccountAssignments\n  method: post\n  operationId: ListAccountAssignments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListAccountsForProvisionedPermissionSet\n  method: post\n  operationId: ListAccountsForProvisionedPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListCustomerManagedPolicyReferencesInPermissionSet\n  method: post\n  operationId: ListCustomerManagedPolicyReferencesInPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListInstances\n  method: post\n  operationId: ListInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /#X-Amz-Target=SWBExternalService.ListManagedPoliciesInPermissionSet\n  method: post\n  operationId: ListManagedPoliciesInPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListPermissionSetProvisioningStatus\n  method: post\n  operationId: ListPermissionSetProvisioningStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListPermissionSets\n  method: post\n  operationId: ListPermissionSets\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListPermissionSetsProvisionedToAccount\n  method: post\n  operationId: ListPermissionSetsProvisionedToAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.ProvisionPermissionSet\n  method: post\n  operationId: ProvisionPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.PutInlinePolicyToPermissionSet\n  method: post\n  operationId: PutInlinePolicyToPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /#X-Amz-Target=SWBExternalService.PutPermissionsBoundaryToPermissionSet\n  method: post\n  operationId: PutPermissionsBoundaryToPermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.UpdateInstanceAccessControlAttributeConfiguration\n  method: post\n  operationId: UpdateInstanceAccessControlAttributeConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=SWBExternalService.UpdatePermissionSet\n  method: post\n  operationId: UpdatePermissionSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/agentic-access/amazon-iam-identity-center-agentic-access.yml
summary_line: 56 operations · 56 acting · 4 human-in-the-loop
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
---
