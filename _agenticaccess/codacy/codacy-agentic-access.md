---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 13
api_specs:
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Organizations API
  slug: organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Repositories API
  slug: repositories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Pull Requests API
  slug: pull-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Coverage API
  slug: coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Security API
  slug: security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
consequence_counts:
  read: 13
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Codacy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Codacy exposes 18 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Codacy
provider_slug: codacy
slug: codacy-agentic-access
source_filename: codacy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/codacy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 13\n    acting: 5\n  by_consequence:\n    read: 13\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/organizations/{provider}\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/organizations/{provider}/{remoteOrganizationName}\n\
  \  method: get\n  operationId: getUserOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories\n  method: get\n  operationId: listOrganizationRepositoriesWithAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}\n  method: get\n  operationId: getRepositoryWithAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/follow\n  method: post\n  operationId: followAddedRepository\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/follow\n  method: delete\n  operationId: unfollowRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/issues/search\n  method: post\n  operationId: searchRepositoryIssues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/issues/{issueId}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/pull-requests\n  method: get\n  operationId: listRepositoryPullRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/pull-requests/{pullRequestNumber}\n  method: get\n  operationId: getRepositoryPullRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/pull-requests/{pullRequestNumber}/issues\n  method: get\n  operationId: listPullRequestIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/pull-requests/{pullRequestNumber}/ai-reviewer/trigger\n  method: post\n  operationId: triggerPullRequestAiReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coverage/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/pull-requests/{pullRequestNumber}\n\
  \  method: get\n  operationId: getRepositoryPullRequestCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coverage/organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/pull-requests/{pullRequestNumber}/files\n  method: get\n  operationId: getRepositoryPullRequestFilesCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/settings/quality/pull-requests\n  method: get\n  operationId: getPullRequestQualitySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/settings/quality/pull-requests\n\
  \  method: put\n  operationId: updatePullRequestQualitySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{provider}/{remoteOrganizationName}/repositories/{repositoryName}/settings/stored-ssh-key\n  method: get\n  operationId: getRepositoryPublicSshKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/agentic-access/codacy-agentic-access.yml
summary_line: 18 operations · 5 acting
tags:
- Code Quality
- Static Analysis
- Security
- Code Coverage
- DevOps
---
