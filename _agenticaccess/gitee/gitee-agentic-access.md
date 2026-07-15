---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 27
api_specs:
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Repositories API
  slug: gitee-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Issues API
  slug: gitee-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Pull Requests API
  slug: gitee-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Users and Organizations API
  slug: gitee-users-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Gists API
  slug: gitee-gists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Enterprises API
  slug: gitee-enterprises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Webhooks API
  slug: gitee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
consequence_counts:
  physical: 1
  read: 27
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gitee Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /repos/{owner}/{repo}/hooks/{id}/tests
operation_count: 41
overview: 'Gitee exposes 41 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 13 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gitee
provider_slug: gitee
slug: gitee-agentic-access
source_filename: gitee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gitee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 27\n    acting: 14\n  by_consequence:\n    read: 27\n    write: 13\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /user\n  method: get\n  operationId: getAuthenticatedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /user/keys\n  method: get\n  operationId: listUserKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n   \
  \ scope:\n    - projects\n- path: /user/keys\n  method: post\n  operationId: createUserKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /user/repos\n  method: get\n  operationId: listUserRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /user/repos\n  method: post\n  operationId: createUserRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    -\
  \ projects\n- path: /repos/{owner}/{repo}\n  method: get\n  operationId: getRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}\n  method: patch\n  operationId: updateRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/branches\n  method: get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/branches\n  method: post\n  operationId: createBranch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/commits\n  method: get\n  operationId: listCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/issues\n  method: get\n  operationId: listRepoIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/issues\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/issues/{number}\n  method: patch\n  operationId: updateIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/issues/{number}/comments\n  method: get\n  operationId: listIssueComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/issues/{number}/comments\n  method: post\n  operationId: createIssueComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/labels\n  method: get\n  operationId: listRepoLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/milestones\n  method: get\n  operationId: listMilestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - projects\n- path: /repos/{owner}/{repo}/pulls\n  method: get\n  operationId: listPullRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/pulls\n  method: post\n  operationId: createPullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/pulls/{number}\n  method: get\n  operationId: getPullRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/pulls/{number}/merge\n  method: get\n\
  \  operationId: isPullRequestMerged\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/pulls/{number}/merge\n  method: put\n  operationId: mergePullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/pulls/{number}/files\n  method: get\n  operationId: listPullRequestFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /user/orgs\n  method: get\n  operationId: listUserOrgs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /orgs/{org}\n  method: get\n  operationId: getOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /orgs/{org}/members\n  method: get\n  operationId: listOrgMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /gists\n  method: get\n  operationId: listGists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /gists\n  method: post\n  operationId: createGist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /gists/{id}\n  method: get\n  operationId: getGist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /gists/{id}\n  method: delete\n  operationId: deleteGist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /user/enterprises\n  method: get\n  operationId: listUserEnterprises\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n    scope:\n    - projects\n- path: /enterprises/{enterprise}\n  method: get\n  operationId: getEnterprise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /enterprises/{enterprise}/members\n  method: get\n  operationId: listEnterpriseMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /enterprises/{enterprise}/members\n  method: post\n  operationId: addEnterpriseMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/hooks\n\
  \  method: get\n  operationId: listRepoHooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/hooks\n  method: post\n  operationId: createRepoHook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - projects\n- path: /repos/{owner}/{repo}/hooks/{id}/tests\n  method: post\n  operationId: testRepoHook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n    scope:\n    - projects\n- path: /search/repositories\n  method: get\n  operationId: searchRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /search/issues\n  method: get\n  operationId: searchIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n- path: /search/users\n  method: get\n  operationId: searchUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - projects\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/agentic-access/gitee-agentic-access.yml
summary_line: 41 operations · 14 acting
tags:
- Code Hosting
- Git
- Git Hosting
- Version Control
- Repositories
- Pull Requests
- Issue Tracking
- DevOps
- Open Source
- China
---
