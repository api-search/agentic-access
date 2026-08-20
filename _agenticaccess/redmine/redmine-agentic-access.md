---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 16
api_specs:
- filename: redmine-attachments-api-openapi.yml
  format: yaml
  label: Redmine Attachments API
  slug: redmine-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-attachments-api-openapi.yml
- filename: redmine-custom-fields-json-api-openapi.yml
  format: yaml
  label: Redmine Custom Fields.json API
  slug: redmine-custom-fields-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-custom-fields-json-api-openapi.yml
- filename: redmine-groups-json-api-openapi.yml
  format: yaml
  label: Redmine Groups.json API
  slug: redmine-groups-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-groups-json-api-openapi.yml
- filename: redmine-issue-statuses-json-api-openapi.yml
  format: yaml
  label: Redmine Issue Statuses.json API
  slug: redmine-issue-statuses-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issue-statuses-json-api-openapi.yml
- filename: redmine-issues-api-openapi.yml
  format: yaml
  label: Redmine Issues API
  slug: redmine-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issues-api-openapi.yml
- filename: redmine-issues-json-api-openapi.yml
  format: yaml
  label: Redmine Issues.json API
  slug: redmine-issues-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issues-json-api-openapi.yml
- filename: redmine-my-api-openapi.yml
  format: yaml
  label: Redmine My API
  slug: redmine-my-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-my-api-openapi.yml
- filename: redmine-projects-api-openapi.yml
  format: yaml
  label: Redmine Projects API
  slug: redmine-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-projects-api-openapi.yml
- filename: redmine-projects-json-api-openapi.yml
  format: yaml
  label: Redmine Projects.json API
  slug: redmine-projects-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-projects-json-api-openapi.yml
- filename: redmine-roles-json-api-openapi.yml
  format: yaml
  label: Redmine Roles.json API
  slug: redmine-roles-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-roles-json-api-openapi.yml
- filename: redmine-time-entries-api-openapi.yml
  format: yaml
  label: Redmine Time Entries API
  slug: redmine-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-time-entries-api-openapi.yml
- filename: redmine-time-entries-json-api-openapi.yml
  format: yaml
  label: Redmine Time Entries.json API
  slug: redmine-time-entries-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-time-entries-json-api-openapi.yml
- filename: redmine-trackers-json-api-openapi.yml
  format: yaml
  label: Redmine Trackers.json API
  slug: redmine-trackers-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-trackers-json-api-openapi.yml
- filename: redmine-uploads-json-api-openapi.yml
  format: yaml
  label: Redmine Uploads.json API
  slug: redmine-uploads-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-uploads-json-api-openapi.yml
- filename: redmine-users-api-openapi.yml
  format: yaml
  label: Redmine Users API
  slug: redmine-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-users-api-openapi.yml
- filename: redmine-users-json-api-openapi.yml
  format: yaml
  label: Redmine Users.json API
  slug: redmine-users-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-users-json-api-openapi.yml
- filename: redmine-wiki-pages-json-api-openapi.yml
  format: yaml
  label: Redmine Wiki Pages.json API
  slug: redmine-wiki-pages-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-wiki-pages-json-api-openapi.yml
consequence_counts:
  read: 16
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Redmine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Redmine exposes 32 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Redmine
provider_slug: redmine
slug: redmine-agentic-access
source_filename: redmine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/redmine-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 16\n    acting: 16\n  by_consequence:\n    read: 16\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /issues.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues.json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /issues/{id}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/{id}.json\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/{id}.json\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /projects.json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{id}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{id}.json\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{id}.json\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users.json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}.json\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}.json\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_entries.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_entries.json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /time_entries/{id}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_entries/{id}.json\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_entries/{id}.json\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{id}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/{id}.json\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads.json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wiki_pages.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wiki_pages.json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue_statuses.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackers.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups.json\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_fields.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /my/account.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/agentic-access/redmine-agentic-access.yml
summary_line: 32 operations · 16 acting
tags:
- Project Management
- Issue Tracking
- Open-Source
- Ruby on Rails
- Bug Tracking
- Time Tracking
---
