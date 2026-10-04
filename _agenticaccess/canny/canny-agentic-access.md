---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 24
api_specs:
- filename: canny-autopilot-api-openapi.yml
  format: yaml
  label: Canny Autopilot API
  slug: canny-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-autopilot-api-openapi.yml
- filename: canny-boards-api-openapi.yml
  format: yaml
  label: Canny Boards API
  slug: canny-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-boards-api-openapi.yml
- filename: canny-categories-api-openapi.yml
  format: yaml
  label: Canny Categories API
  slug: canny-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-categories-api-openapi.yml
- filename: canny-changelogentries-api-openapi.yml
  format: yaml
  label: Canny ChangelogEntries API
  slug: canny-changelogentries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-changelogentries-api-openapi.yml
- filename: canny-comments-api-openapi.yml
  format: yaml
  label: Canny Comments API
  slug: canny-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-comments-api-openapi.yml
- filename: canny-companies-api-openapi.yml
  format: yaml
  label: Canny Companies API
  slug: canny-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-companies-api-openapi.yml
- filename: canny-groups-api-openapi.yml
  format: yaml
  label: Canny Groups API
  slug: canny-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-groups-api-openapi.yml
- filename: canny-ideas-api-openapi.yml
  format: yaml
  label: Canny Ideas API
  slug: canny-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-ideas-api-openapi.yml
- filename: canny-insights-api-openapi.yml
  format: yaml
  label: Canny Insights API
  slug: canny-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-insights-api-openapi.yml
- filename: canny-opportunities-api-openapi.yml
  format: yaml
  label: Canny Opportunities API
  slug: canny-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-opportunities-api-openapi.yml
- filename: canny-posts-api-openapi.yml
  format: yaml
  label: Canny Posts API
  slug: canny-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-posts-api-openapi.yml
- filename: canny-statuschanges-api-openapi.yml
  format: yaml
  label: Canny StatusChanges API
  slug: canny-statuschanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-statuschanges-api-openapi.yml
- filename: canny-tags-api-openapi.yml
  format: yaml
  label: Canny Tags API
  slug: canny-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-tags-api-openapi.yml
- filename: canny-users-api-openapi.yml
  format: yaml
  label: Canny Users API
  slug: canny-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-users-api-openapi.yml
- filename: canny-votes-api-openapi.yml
  format: yaml
  label: Canny Votes API
  slug: canny-votes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-votes-api-openapi.yml
consequence_counts:
  read: 24
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Canny Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 51
overview: 'Canny exposes 51 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 27 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Canny
provider_slug: canny
slug: canny-agentic-access
source_filename: canny-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/canny-autopilot-api-openapi.yml, openapi/canny-boards-api-openapi.yml, openapi/canny-categories-api-openapi.yml,\n  openapi/canny-changelogentries-api-openapi.yml, openapi/canny-comments-api-openapi.yml, openapi/canny-companies-api-openapi.yml,\n  openapi/canny-groups-api-openapi.yml, openapi/canny-ideas-api-openapi.yml, openapi/canny-insights-api-openapi.yml,\n  openapi/canny-opportunities-api-openapi.yml, openapi/canny-posts-api-openapi.yml, openapi/canny-statuschanges-api-openapi.yml,\n  openapi/canny-tags-api-openapi.yml, openapi/canny-users-api-openapi.yml, openapi/canny-votes-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    acting: 27\n\
  \    connected: 24\n  by_consequence:\n    write: 27\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /autopilot/enqueue_feedback\n  method: post\n  operationId: postAutopilotEnqueueFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/retrieve\n  method: post\n  operationId: postBoardsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/list\n  method: post\n  operationId: postBoardsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/retrieve\n  method: post\n  operationId: postCategoriesRetrieve\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/list\n  method: post\n  operationId: postCategoriesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/create\n  method: post\n  operationId: postCategoriesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories/delete\n  method: post\n  operationId: postCategoriesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entries/create\n  method: post\n  operationId: postEntriesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entries/list\n  method: post\n  operationId: postEntriesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments/retrieve\n  method: post\n  operationId: postCommentsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments/list\n  method: post\n  operationId: postCommentsList\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments/create\n  method: post\n  operationId: postCommentsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments/delete\n  method: post\n  operationId: postCommentsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/list\n  method: post\n  operationId: postCompaniesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /companies/update\n  method: post\n  operationId: postCompaniesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/delete\n  method: post\n  operationId: postCompaniesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/list\n  method: post\n  operationId: postGroupsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/retrieve\n  method: post\n  operationId:\
  \ postGroupsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ideas/list\n  method: post\n  operationId: postIdeasList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ideas/retrieve\n  method: post\n  operationId: postIdeasRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ideas/merge\n  method: post\n  operationId: postIdeasMerge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ideas/delete\n  method: post\n  operationId:\
  \ postIdeasDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/list\n  method: post\n  operationId: postInsightsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/retrieve\n  method: post\n  operationId: postInsightsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/list\n  method: post\n  operationId: postOpportunitiesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/retrieve\n  method:\
  \ post\n  operationId: postPostsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/list\n  method: post\n  operationId: postPostsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/create\n  method: post\n  operationId: postPostsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/change_board\n  method: post\n  operationId: postPostsChangeBoard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/change_category\n  method: post\n  operationId: postPostsChangeCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/change_status\n  method: post\n  operationId: postPostsChangeStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/merge\n  method: post\n  operationId: postPostsMerge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/add_tag\n  method: post\n  operationId: postPostsAddTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/remove_tag\n  method: post\n  operationId: postPostsRemoveTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/update\n  method: post\n  operationId: postPostsUpdate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/delete\n  method: post\n  operationId: postPostsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/link_jira\n  method: post\n  operationId: postPostsLinkJira\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/unlink_jira\n  method: post\n  operationId: postPostsUnlinkJira\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status_changes/list\n  method: post\n  operationId: postStatusChangesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/retrieve\n  method: post\n  operationId: postTagsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/list\n  method: post\n  operationId: postTagsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/create\n  method: post\n  operationId: postTagsCreate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/list\n  method: post\n  operationId: postUsersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/retrieve\n  method: post\n  operationId: postUsersRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/create_or_update\n  method: post\n  operationId: postUsersCreateOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/delete\n  method: post\n  operationId: postUsersDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/remove_from_company\n  method: post\n  operationId: postUsersRemoveFromCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /votes/retrieve\n  method: post\n  operationId: postVotesRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /votes/list\n  method: post\n  operationId: postVotesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /votes/create\n  method: post\n  operationId: postVotesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /votes/delete\n  method: post\n  operationId: postVotesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/agentic-access/canny-agentic-access.yml
summary_line: 51 operations · 27 acting
tags:
- Customer Feedback
- Product Management
- Feature Requests
- Roadmaps
- Changelog
- Voice of Customer
- Software-as-a-Service
---
