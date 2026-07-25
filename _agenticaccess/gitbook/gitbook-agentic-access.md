---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 32
api_specs:
- filename: gitbook-change-request-content-api-openapi.yml
  format: yaml
  label: GitBook Change Request Content API
  slug: gitbook-change-request-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-request-content-api-openapi.yml
- filename: gitbook-change-request-reviewers-api-openapi.yml
  format: yaml
  label: GitBook Change Request Reviewers API
  slug: gitbook-change-request-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-request-reviewers-api-openapi.yml
- filename: gitbook-change-requests-api-openapi.yml
  format: yaml
  label: GitBook Change Requests API
  slug: gitbook-change-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-requests-api-openapi.yml
- filename: gitbook-collections-api-openapi.yml
  format: yaml
  label: GitBook Collections API
  slug: gitbook-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-collections-api-openapi.yml
- filename: gitbook-custom-hostnames-api-openapi.yml
  format: yaml
  label: GitBook Custom Hostnames API
  slug: gitbook-custom-hostnames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-custom-hostnames-api-openapi.yml
- filename: gitbook-docs-sites-api-openapi.yml
  format: yaml
  label: GitBook Docs Sites API
  slug: gitbook-docs-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-docs-sites-api-openapi.yml
- filename: gitbook-imports-api-openapi.yml
  format: yaml
  label: GitBook Imports API
  slug: gitbook-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-imports-api-openapi.yml
- filename: gitbook-integrations-api-openapi.yml
  format: yaml
  label: GitBook Integrations API
  slug: gitbook-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-integrations-api-openapi.yml
- filename: gitbook-openapi-specs-api-openapi.yml
  format: yaml
  label: GitBook OpenAPI Specs API
  slug: gitbook-openapi-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-openapi-specs-api-openapi.yml
- filename: gitbook-organization-members-api-openapi.yml
  format: yaml
  label: GitBook Organization Members API
  slug: gitbook-organization-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organization-members-api-openapi.yml
- filename: gitbook-organization-teams-api-openapi.yml
  format: yaml
  label: GitBook Organization Teams API
  slug: gitbook-organization-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organization-teams-api-openapi.yml
- filename: gitbook-organizations-api-openapi.yml
  format: yaml
  label: GitBook Organizations API
  slug: gitbook-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organizations-api-openapi.yml
- filename: gitbook-search-api-openapi.yml
  format: yaml
  label: GitBook Search API
  slug: gitbook-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-search-api-openapi.yml
- filename: gitbook-site-spaces-api-openapi.yml
  format: yaml
  label: GitBook Site Spaces API
  slug: gitbook-site-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-site-spaces-api-openapi.yml
- filename: gitbook-space-content-api-openapi.yml
  format: yaml
  label: GitBook Space Content API
  slug: gitbook-space-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-space-content-api-openapi.yml
- filename: gitbook-space-users-api-openapi.yml
  format: yaml
  label: GitBook Space Users API
  slug: gitbook-space-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-space-users-api-openapi.yml
- filename: gitbook-spaces-api-openapi.yml
  format: yaml
  label: GitBook Spaces API
  slug: gitbook-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-spaces-api-openapi.yml
- filename: gitbook-urls-api-openapi.yml
  format: yaml
  label: GitBook URLs API
  slug: gitbook-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-urls-api-openapi.yml
- filename: gitbook-users-api-openapi.yml
  format: yaml
  label: GitBook Users API
  slug: gitbook-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-users-api-openapi.yml
consequence_counts:
  physical: 1
  read: 32
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gitbook Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spaces/{spaceId}/transfer
operation_count: 64
overview: 'GitBook exposes 64 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 31 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitBook
provider_slug: gitbook
slug: gitbook-agentic-access
source_filename: gitbook-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gitbook-gitbook-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    connected: 32\n    acting: 32\n  by_consequence:\n    read: 32\n    write: 31\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /user\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: get\n  operationId: getUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs\n  method:\
  \ get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}\n  method: patch\n  operationId: updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/members\n  method: get\n  operationId: listOrganizationMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /orgs/{organizationId}/members/{userId}\n  method: get\n  operationId: getOrganizationMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/members/{userId}\n  method: patch\n  operationId: updateOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/members/{userId}\n  method: delete\n  operationId: removeOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /orgs/{organizationId}/teams\n  method: get\n  operationId: listOrganizationTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/teams/{teamId}\n  method: get\n  operationId: getOrganizationTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/spaces\n  method: get\n  operationId: listSpacesInOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/spaces\n  method: post\n  operationId: createSpaceInOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}\n  method: patch\n  operationId: updateSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}\n  method: delete\n  operationId: deleteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /spaces/{spaceId}/duplicate\n  method: post\n  operationId: duplicateSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/move\n  method: post\n  operationId: moveSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/transfer\n  method: post\n  operationId: transferSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/restore\n  method: post\n  operationId: restoreSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/permissions/users\n  method: get\n  operationId: listSpaceUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/permissions/users/{userId}\n  method: patch\n  operationId: updateSpaceUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/permissions/users/{userId}\n  method: delete\n  operationId: removeSpaceUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/content\n  method: get\n  operationId: getSpaceContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/content/page/{pageId}\n  method: get\n  operationId: getPageInSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/content/page/{pageId}\n\
  \  method: put\n  operationId: updatePageInSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/content/files\n  method: get\n  operationId: listFilesInSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/collections\n  method: get\n  operationId: listCollectionsInOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collectionId}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: delete\n  operationId: deleteCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/change-requests\n  method: get\n  operationId: listChangeRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /spaces/{spaceId}/change-requests\n  method: post\n  operationId: createChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}\n  method: get\n  operationId: getChangeRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}\n  method: patch\n  operationId: updateChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}/merge\n  method: post\n  operationId: mergeChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}/content\n  method: get\n  operationId: getChangeRequestContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}/content/page/{pageId}\n  method: get\n  operationId: getPageInChangeRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}/content/page/{pageId}\n\
  \  method: put\n  operationId: updatePageInChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}/reviewers\n  method: get\n  operationId: listChangeRequestReviewers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/change-requests/{changeRequestId}/reviewers\n  method: post\n  operationId: requestChangeRequestReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /orgs/{organizationId}/sites\n  method: get\n  operationId: listDocsSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/sites\n  method: post\n  operationId: createDocsSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}\n  method: get\n  operationId: getDocsSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/sites/{siteId}\n  method: patch\n  operationId: updateDocsSite\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}\n  method: delete\n  operationId: deleteDocsSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}/site-spaces\n  method: get\n  operationId: listSiteSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/sites/{siteId}/site-spaces\n  method: post\n  operationId: addSiteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}/site-spaces/{siteSpaceId}\n  method: patch\n  operationId: updateSiteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}/site-spaces/{siteSpaceId}\n  method: delete\n  operationId: removeSiteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /orgs/{organizationId}/sites/{siteId}/site-spaces/{siteSpaceId}/move\n  method: post\n  operationId: moveSiteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}/ask\n  method: post\n  operationId: askSiteAI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/search\n  method: get\n  operationId: searchOrganizationContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /orgs/{organizationId}/openapi\n  method: get\n  operationId: listOpenAPISpecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/openapi\n  method: post\n  operationId: uploadOpenAPISpec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/openapi/{specSlug}\n  method: get\n  operationId: getOpenAPISpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/integrations/{integrationId}\n  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/import/content\n  method: post\n  operationId: importContentToSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /urls/content\n  method: get\n  operationId: resolveContentURL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /urls/embed\n  method: get\n  operationId:\
  \ resolveEmbedURL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/sites/{siteId}/custom-hostname\n  method: get\n  operationId: getCustomHostname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{organizationId}/sites/{siteId}/custom-hostname\n  method: put\n  operationId: setCustomHostname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{organizationId}/sites/{siteId}/custom-hostname\n  method: delete\n  operationId: removeCustomHostname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/agentic-access/gitbook-agentic-access.yml
summary_line: 64 operations · 32 acting
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
---
