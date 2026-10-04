---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 5
api_specs:
- filename: amazon-codestar-aws-codestar-api-openapi.yml
  format: yaml
  label: Amazon CodeStar AWS CodeStar API
  slug: amazon-codestar-aws-codestar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/openapi/amazon-codestar-aws-codestar-api-openapi.yml
consequence_counts:
  read: 5
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Codestar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Amazon CodeStar exposes 18 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
slug: amazon-codestar-agentic-access
source_filename: amazon-codestar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-codestar-x-amz-target-codestar-20170419-associateteammember-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-createproject-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-createuserprofile-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-deleteproject-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-deleteuserprofile-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-describeproject-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-describeuserprofile-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-disassociateteammember-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-listprojects-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-listresources-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-listtagsforproject-api-openapi.yml,\n\
  \  openapi/amazon-codestar-x-amz-target-codestar-20170419-listteammembers-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-listuserprofiles-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-tagproject-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-untagproject-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-updateproject-api-openapi.yml, openapi/amazon-codestar-x-amz-target-codestar-20170419-updateteammember-api-openapi.yml,\n  openapi/amazon-codestar-x-amz-target-codestar-20170419-updateuserprofile-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 13\n    connected: 5\n  by_consequence:\n    write: 13\n \
  \   read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /#X-Amz-Target=CodeStar_20170419.AssociateTeamMember\n  method: post\n  operationId: AssociateTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.CreateProject\n  method: post\n  operationId: CreateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.CreateUserProfile\n  method: post\n  operationId: CreateUserProfile\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.DeleteProject\n  method: post\n  operationId: DeleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.DeleteUserProfile\n  method: post\n  operationId: DeleteUserProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.DescribeProject\n\
  \  method: post\n  operationId: DescribeProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.DescribeUserProfile\n  method: post\n  operationId: DescribeUserProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.DisassociateTeamMember\n  method: post\n  operationId: DisassociateTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.ListProjects\n  method: post\n  operationId: ListProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeStar_20170419.ListResources\n  method: post\n  operationId: ListResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeStar_20170419.ListTagsForProject\n  method: post\n  operationId: ListTagsForProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeStar_20170419.ListTeamMembers\n  method: post\n  operationId: ListTeamMembers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeStar_20170419.ListUserProfiles\n  method: post\n  operationId: ListUserProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeStar_20170419.TagProject\n  method: post\n  operationId: TagProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.UntagProject\n  method: post\n  operationId: UntagProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.UpdateProject\n  method: post\n  operationId: UpdateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.UpdateTeamMember\n  method: post\n  operationId: UpdateTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeStar_20170419.UpdateUserProfile\n  method: post\n  operationId: UpdateUserProfile\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/agentic-access/amazon-codestar-agentic-access.yml
summary_line: 18 operations · 13 acting
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
---
