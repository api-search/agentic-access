---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 25
api_specs:
- filename: bokendell-com-activity-api-openapi.yml
  format: yaml
  label: Bo Kendell Activity API
  slug: bokendell-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-activity-api-openapi.yml
- filename: bokendell-com-ai-api-openapi.yml
  format: yaml
  label: Bo Kendell AI API
  slug: bokendell-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-ai-api-openapi.yml
- filename: bokendell-com-contacts-api-openapi.yml
  format: yaml
  label: Bo Kendell Contacts API
  slug: bokendell-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-contacts-api-openapi.yml
- filename: bokendell-com-events-api-openapi.yml
  format: yaml
  label: Bo Kendell Events API
  slug: bokendell-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-events-api-openapi.yml
- filename: bokendell-com-health-api-openapi.yml
  format: yaml
  label: Bo Kendell Health API
  slug: bokendell-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-health-api-openapi.yml
- filename: bokendell-com-profile-api-openapi.yml
  format: yaml
  label: Bo Kendell Profile API
  slug: bokendell-com-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-profile-api-openapi.yml
- filename: bokendell-com-projects-api-openapi.yml
  format: yaml
  label: Bo Kendell Projects API
  slug: bokendell-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-projects-api-openapi.yml
- filename: bokendell-com-resume-api-openapi.yml
  format: yaml
  label: Bo Kendell Resume API
  slug: bokendell-com-resume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-resume-api-openapi.yml
- filename: bokendell-com-social-links-api-openapi.yml
  format: yaml
  label: Bo Kendell Social Links API
  slug: bokendell-com-social-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-social-links-api-openapi.yml
- filename: bokendell-com-tags-api-openapi.yml
  format: yaml
  label: Bo Kendell Tags API
  slug: bokendell-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-tags-api-openapi.yml
- filename: bokendell-com-technologies-api-openapi.yml
  format: yaml
  label: Bo Kendell Technologies API
  slug: bokendell-com-technologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-technologies-api-openapi.yml
- filename: bokendell-com-writing-api-openapi.yml
  format: yaml
  label: Bo Kendell Writing API
  slug: bokendell-com-writing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-writing-api-openapi.yml
consequence_counts:
  physical: 1
  read: 25
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bokendell Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/ai/tools/send-email-to-bo
operation_count: 30
overview: 'Bo Kendell exposes 30 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bo Kendell
provider_slug: bokendell-com
slug: bokendell-com-agentic-access
source_filename: bokendell-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bokendell-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 25\n    acting: 5\n  by_consequence:\n    read: 25\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/activity\n  method: get\n  operationId: v1.activity.getCombined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity/github/contributions\n  method: get\n  operationId: v1.activity.getGithubContributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity/github/events\n  method: get\n  operationId: v1.activity.getGithubEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity/leetcode\n  method: get\n  operationId: v1.activity.getLeetcodeStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity/latest-commit\n  method: get\n  operationId: v1.activity.getLatestCommit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity/weekly-summary\n  method: get\n  operationId: v1.activity.getWeeklySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/ai/chat/stream\n  method: post\n  operationId: v1.ai.chat.stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/demo/homepage\n  method: post\n  operationId: v1.ai.demo.homepage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/demo/mcp-trace\n  method: post\n  operationId: v1.ai.demo.mcpTrace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/tools\n  method: get\n  operationId: v1.ai.tools.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/tools/send-email-to-bo\n  method: post\n  operationId: v1.ai.tools.sendEmailToBo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contacts\n  method: post\n  operationId: v1.contacts.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/events\n  method: get\n  operationId: v1.events.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events/{id}\n  method: get\n  operationId: v1.events.getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: v1.health.check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts\n  method: get\n  operationId: v1.posts.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts/{slug}\n  method:\
  \ get\n  operationId: v1.posts.getBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/profiles\n  method: get\n  operationId: v1.profile.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/profiles/{id}\n  method: get\n  operationId: v1.profile.getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects\n  method: get\n  operationId: v1.projects.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/featured\n  method: get\n  operationId: v1.projects.listFeatured\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/archive\n  method: get\n  operationId: v1.projects.listArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/{slug}\n  method: get\n  operationId: v1.projects.getBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/resume\n  method: get\n  operationId: v1.resume.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/social-links\n  method: get\n  operationId: v1.socialLinks.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/social-links/{id}\n\
  \  method: get\n  operationId: v1.socialLinks.getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tags\n  method: get\n  operationId: v1.tags.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/technologies\n  method: get\n  operationId: v1.technologies.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/technologies/featured\n  method: get\n  operationId: v1.technologies.getFeatured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/technologies/{id}\n  method: get\n  operationId: v1.technologies.getById\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bokendell-com/agentic-access/bokendell-com-agentic-access.yml
summary_line: 30 operations · 5 acting
tags:
- Software Engineer
- Backend
- Artificial Intelligence
- OpenAPI
- MCP
---
