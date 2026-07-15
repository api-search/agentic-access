---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 14
api_specs:
- filename: git.json
  format: json
  label: Azure DevOps Services REST API - Git
  slug: azure-devops-services-rest-api-git
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/git/7.1/git.json
- filename: tfvc.json
  format: json
  label: Azure DevOps Services REST API - TFVC
  slug: azure-devops-services-rest-api-tfvc
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/tfvc/7.1/tfvc.json
- filename: policy.json
  format: json
  label: Azure DevOps Services REST API - Policy
  slug: azure-devops-services-rest-api-policy
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/policy/7.1/policy.json
consequence_counts:
  read: 14
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Azure Repo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Azure Repos exposes 24 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azure Repos
provider_slug: microsoft-azure-repo
slug: microsoft-azure-repo-agentic-access
source_filename: microsoft-azure-repo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/azure-repo-git-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 14\n    acting: 10\n  by_consequence:\n    read: 14\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /git/repositories\n  method: get\n  operationId: repositories_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories\n  method: post\n  operationId: repositories_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}\n  method: get\n  operationId: repositories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}\n  method: patch\n  operationId: repositories_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}\n  method: delete\n  operationId: repositories_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pullrequests\n  method: get\n  operationId: pullRequests_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/pullrequests\n  method: post\n  operationId: pullRequests_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}\n  method: get\n  operationId: pullRequests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}\n\
  \  method: patch\n  operationId: pullRequests_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}/reviewers\n  method: get\n  operationId: pullRequestReviewers_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}/reviewers/{reviewerId}\n  method: put\n  operationId: pullRequestReviewers_createOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}/reviewers/{reviewerId}\n  method: delete\n  operationId: pullRequestReviewers_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}/threads\n  method: get\n  operationId: pullRequestThreads_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}/threads\n  method: post\n  operationId: pullRequestThreads_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pullrequests/{pullRequestId}/commits\n  method: get\n  operationId: pullRequestCommits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/commits\n  method: get\n  operationId: commits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/commits/{commitId}\n  method: get\n  operationId: commits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/refs\n\
  \  method: get\n  operationId: refs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/refs\n  method: post\n  operationId: refs_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pushes\n  method: get\n  operationId: pushes_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/pushes\n  method: post\n  operationId: pushes_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /git/repositories/{repositoryId}/pushes/{pushId}\n  method: get\n  operationId: pushes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/items\n  method: get\n  operationId: items_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /git/repositories/{repositoryId}/stats/branches\n  method: get\n  operationId: stats_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/agentic-access/microsoft-azure-repo-agentic-access.yml
summary_line: 24 operations · 10 acting
tags:
- DevOps
- Git
- Repositories
- Source Control
- TFVC
- Version Control
---
