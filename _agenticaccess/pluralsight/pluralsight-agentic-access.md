---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 17
api_specs:
- filename: pluralsight-catalog-api-openapi.yml
  format: yaml
  label: Pluralsight Catalog API
  slug: pluralsight-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-catalog-api-openapi.yml
- filename: pluralsight-coding-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Coding Metrics API
  slug: pluralsight-coding-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-coding-metrics-api-openapi.yml
- filename: pluralsight-collaboration-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Collaboration Metrics API
  slug: pluralsight-collaboration-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-collaboration-metrics-api-openapi.yml
- filename: pluralsight-commits-api-openapi.yml
  format: yaml
  label: Pluralsight Commits API
  slug: pluralsight-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-commits-api-openapi.yml
- filename: pluralsight-dora-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight DORA Metrics API
  slug: pluralsight-dora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-dora-metrics-api-openapi.yml
- filename: pluralsight-graphql-api-openapi.yml
  format: yaml
  label: Pluralsight GraphQL API
  slug: pluralsight-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-graphql-api-openapi.yml
- filename: pluralsight-integrations-api-openapi.yml
  format: yaml
  label: Pluralsight Integrations API
  slug: pluralsight-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-integrations-api-openapi.yml
- filename: pluralsight-licensing-api-openapi.yml
  format: yaml
  label: Pluralsight Licensing API
  slug: pluralsight-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-licensing-api-openapi.yml
- filename: pluralsight-pull-requests-api-openapi.yml
  format: yaml
  label: Pluralsight Pull Requests API
  slug: pluralsight-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-pull-requests-api-openapi.yml
- filename: pluralsight-reports-api-openapi.yml
  format: yaml
  label: Pluralsight Reports API
  slug: pluralsight-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-reports-api-openapi.yml
- filename: pluralsight-repos-api-openapi.yml
  format: yaml
  label: Pluralsight Repos API
  slug: pluralsight-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-repos-api-openapi.yml
- filename: pluralsight-teams-api-openapi.yml
  format: yaml
  label: Pluralsight Teams API
  slug: pluralsight-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-teams-api-openapi.yml
- filename: pluralsight-tickets-api-openapi.yml
  format: yaml
  label: Pluralsight Tickets API
  slug: pluralsight-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-tickets-api-openapi.yml
- filename: pluralsight-users-api-openapi.yml
  format: yaml
  label: Pluralsight Users API
  slug: pluralsight-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-users-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Pluralsight Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /graphql
operation_count: 36
overview: 'Pluralsight exposes 36 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 18 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pluralsight
provider_slug: pluralsight
slug: pluralsight-agentic-access
source_filename: pluralsight-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/channels.yml, openapi/content-catalog.yml, openapi/content-progress.yml, openapi/content-slug.yml,\n  openapi/course-catalog.yml, openapi/course-daily-usage.yml, openapi/course-progress.yml, openapi/flow-coding-metrics.yml,\n  openapi/flow-collaboration-metrics.yml, openapi/flow-commits.yml, openapi/flow-dora-metrics.yml,\n  openapi/flow-integrations.yml, openapi/flow-pull-requests.yml, openapi/flow-repos.yml, openapi/flow-teams.yml,\n  openapi/flow-tickets.yml, openapi/flow-users.yml, openapi/labs.yml, openapi/learning-paths.yml,\n  openapi/licensing-rest.yml, openapi/plan-info.yml, openapi/practice-exams.yml, openapi/programs.yml,\n  openapi/public-course-catalog-rest.yml, openapi/reports-rest.yml, openapi/role-iq.yml, openapi/skills-assessment.yml,\n  openapi/tags.yml, openapi/teams.yml, openapi/user-management.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the\
  \ OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 19\n    connected: 17\n  by_consequence:\n    write: 18\n    read: 17\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /graphql\n  method: post\n  operationId: manageChannels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryContentCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryContentProgress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryContentSlugs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryCourseCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryCourseDailyUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryCourseProgress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collaboration/code/metrics\n  method: get\n  operationId: getCodingMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /collaboration/pullrequest/metrics\n  method: get\n  operationId: getCollaborationMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commits\n  method: get\n  operationId: getCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dora/build-release\n  method: get\n  operationId: getDoraMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pull-requests\n  method: get\n  operationId: getPullRequests\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos\n  method: get\n  operationId: getRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets\n  method: get\n  operationId: getTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: put\n  operationId: updateUsers\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryLabs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryLearningPaths\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invitations\n  method: get\n \
  \ operationId: listInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: post\n  operationId: createInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graphql\n  method: post\n  operationId: queryPlanInfo\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryPracticeExams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryPrograms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /courses\n  method: get\n  operationId: getCourseCatalog\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: downloadUserReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /course-completion\n  method: get\n  operationId: downloadCourseCompletionReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /course-usage\n  method: get\n  operationId: downloadCourseUsageReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graphql\n  method: post\n  operationId: manageRoleIQ\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: querySkillsAssessment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /graphql\n  method: post\n  operationId: queryTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: manageTeams\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: manageUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/agentic-access/pluralsight-agentic-access.yml
summary_line: 36 operations · 19 acting · 1 human-in-the-loop
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
---
