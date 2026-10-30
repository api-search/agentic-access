---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 26
api_specs:
- filename: codeberg-miscellaneous-api-openapi.yml
  format: yaml
  label: Codeberg Miscellaneous API
  slug: codeberg-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-miscellaneous-api-openapi.yml
- filename: codeberg-activitypub-api-openapi.yml
  format: yaml
  label: Codeberg Activitypub API
  slug: codeberg-activitypub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-activitypub-api-openapi.yml
- filename: codeberg-admin-api-openapi.yml
  format: yaml
  label: Codeberg Admin API
  slug: codeberg-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-admin-api-openapi.yml
- filename: codeberg-issue-api-openapi.yml
  format: yaml
  label: Codeberg Issue API
  slug: codeberg-issue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-issue-api-openapi.yml
- filename: codeberg-notification-api-openapi.yml
  format: yaml
  label: Codeberg Notification API
  slug: codeberg-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-notification-api-openapi.yml
- filename: codeberg-organization-api-openapi.yml
  format: yaml
  label: Codeberg Organization API
  slug: codeberg-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-organization-api-openapi.yml
- filename: codeberg-package-api-openapi.yml
  format: yaml
  label: Codeberg Package API
  slug: codeberg-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-package-api-openapi.yml
- filename: codeberg-repository-api-openapi.yml
  format: yaml
  label: Codeberg Repository API
  slug: codeberg-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-repository-api-openapi.yml
- filename: codeberg-settings-api-openapi.yml
  format: yaml
  label: Codeberg Settings API
  slug: codeberg-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-settings-api-openapi.yml
- filename: codeberg-user-api-openapi.yml
  format: yaml
  label: Codeberg User API
  slug: codeberg-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-user-api-openapi.yml
consequence_counts:
  read: 26
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Codeberg Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'Codeberg exposes 44 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Codeberg
provider_slug: codeberg
slug: codeberg-agentic-access
source_filename: codeberg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/codeberg-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 26\n    acting: 18\n  by_consequence:\n    read: 26\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/search\n  method: get\n  operationId: repoSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}\n  method: get\n  operationId:\
  \ repoGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}\n  method: patch\n  operationId: repoEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}\n  method: delete\n  operationId: repoDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/repos\n  method: get\n  operationId: userCurrentListRepos\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/repos\n  method: post\n  operationId: createCurrentUserRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/branches\n  method: get\n  operationId: repoListBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/branches\n  method: post\n  operationId: repoCreateBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /repos/{owner}/{repo}/tags\n  method: get\n  operationId: repoListTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/issues/search\n  method: get\n  operationId: issueSearchIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/issues\n  method: get\n  operationId: issueListIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/issues\n  method: post\n  operationId: issueCreateIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/issues/{index}\n  method: get\n  operationId: issueGetIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/issues/{index}\n  method: patch\n  operationId: issueEditIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/issues/{index}/comments\n  method: get\n  operationId: issueGetComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/issues/{index}/comments\n  method: post\n\
  \  operationId: issueCreateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/pulls\n  method: get\n  operationId: repoListPullRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/pulls\n  method: post\n  operationId: repoCreatePullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/pulls/{index}\n  method: get\n  operationId: repoGetPullRequest\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/pulls/{index}\n  method: patch\n  operationId: repoEditPullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/pulls/{index}/merge\n  method: get\n  operationId: repoPullRequestIsMerged\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/pulls/{index}/merge\n  method: post\n  operationId: repoMergePullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/releases\n  method: get\n  operationId: repoListReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/releases\n  method: post\n  operationId: repoCreateRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/releases/latest\n  method: get\n  operationId: repoGetLatestRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /repos/{owner}/{repo}/releases/{id}\n  method: get\n  operationId: repoGetRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/releases/{id}\n  method: patch\n  operationId: repoEditRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/releases/{id}\n  method: delete\n  operationId: repoDeleteRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/contents/{filepath}\n\
  \  method: get\n  operationId: repoGetContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/contents/{filepath}\n  method: post\n  operationId: repoCreateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/contents/{filepath}\n  method: put\n  operationId: repoUpdateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/contents/{filepath}\n  method:\
  \ delete\n  operationId: repoDeleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/raw/{filepath}\n  method: get\n  operationId: repoGetRawFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/commits\n  method: get\n  operationId: repoGetAllCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/git/trees/{sha}\n  method: get\n  operationId: getTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /user\n  method: get\n  operationId: userGetCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/search\n  method: get\n  operationId: userSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}\n  method: get\n  operationId: userGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}/repos\n  method: get\n  operationId: userListRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}\n  method: get\n  operationId: orgGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}\n  method: patch\n  operationId: orgEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/repos\n  method: get\n  operationId: orgListRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repos\n  method: post\n  operationId: createOrgRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/agentic-access/codeberg-agentic-access.yml
summary_line: 44 operations · 18 acting
tags:
- Code Hosting
- Version Control
- Git Hosting
- Repositories
- Pull Requests
- Issue Tracking
- Open Source
- Forgejo
- Non-Profit
---
