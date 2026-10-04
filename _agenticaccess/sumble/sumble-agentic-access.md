---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 14
api_specs:
- filename: sumble-contact-lists-api-openapi.yml
  format: yaml
  label: Sumble Contact Lists API
  slug: sumble-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-contact-lists-api-openapi.yml
- filename: sumble-jobs-api-openapi.yml
  format: yaml
  label: Sumble Jobs API
  slug: sumble-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-jobs-api-openapi.yml
- filename: sumble-organization-lists-api-openapi.yml
  format: yaml
  label: Sumble Organization Lists API
  slug: sumble-organization-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organization-lists-api-openapi.yml
- filename: sumble-organizations-api-openapi.yml
  format: yaml
  label: Sumble Organizations API
  slug: sumble-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organizations-api-openapi.yml
- filename: sumble-people-api-openapi.yml
  format: yaml
  label: Sumble People API
  slug: sumble-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-people-api-openapi.yml
- filename: sumble-projects-api-openapi.yml
  format: yaml
  label: Sumble Projects API
  slug: sumble-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-projects-api-openapi.yml
- filename: sumble-signals-api-openapi.yml
  format: yaml
  label: Sumble Signals API
  slug: sumble-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-signals-api-openapi.yml
- filename: sumble-support-api-openapi.yml
  format: yaml
  label: Sumble Support API
  slug: sumble-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-support-api-openapi.yml
- filename: sumble-teams-api-openapi.yml
  format: yaml
  label: Sumble Teams API
  slug: sumble-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-teams-api-openapi.yml
- filename: sumble-technologies-api-openapi.yml
  format: yaml
  label: Sumble Technologies API
  slug: sumble-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-technologies-api-openapi.yml
consequence_counts:
  read: 14
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sumble Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Sumble exposes 26 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sumble
provider_slug: sumble
slug: sumble-agentic-access
source_filename: sumble-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/sumble-contact-lists-api-openapi.yml, openapi/sumble-jobs-api-openapi.yml, openapi/sumble-organization-lists-api-openapi.yml,\n  openapi/sumble-organizations-api-openapi.yml, openapi/sumble-people-api-openapi.yml, openapi/sumble-projects-api-openapi.yml,\n  openapi/sumble-signals-api-openapi.yml, openapi/sumble-support-api-openapi.yml, openapi/sumble-teams-api-openapi.yml,\n  openapi/sumble-technologies-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 14\n    acting: 12\n  by_consequence:\n    read: 14\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v9/contact-lists\n  method: get\n  operationId: list_contact_lists__api_version__contact_lists_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/contact-lists\n  method: post\n  operationId: create_contact_list__api_version__contact_lists_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/contact-lists/{list_id}/people\n  method: post\n  operationId: add_contacts_to_list__api_version__contact_lists__list_id__people_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/contact-lists/{list_id}\n  method:\
  \ get\n  operationId: get_contact_list__api_version__contact_lists__list_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/jobs/title-lookup\n  method: post\n  operationId: lookup_job_titles__api_version__jobs_title_lookup_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/jobs\n  method: post\n  operationId: enrich_jobs_unified__api_version__jobs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/organization-lists\n  method: get\n  operationId: list_organization_lists__api_version__organization_lists_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/organization-lists\n  method: post\n  operationId: create_organization_list__api_version__organization_lists_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/organization-lists/{list_id}\n  method: get\n  operationId: get_organization_list__api_version__organization_lists__list_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/organization-lists/{list_id}/deleted\n  method: post\n  operationId: set_organization_list_deleted__api_version__organization_lists__list_id__deleted_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/organization-lists/{list_id}/organizations\n  method: post\n  operationId: add_organizations_to_list__api_version__organization_lists__list_id__organizations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/organization-lists/{list_id}/signals\n  method: post\n  operationId: set_organization_list_signals__api_version__organization_lists__list_id__signals_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/organizations\n  method: post\n  operationId: enrich_organizations_unified__api_version__organizations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/organizations/{organization_id}/intelligence-brief\n  method: get\n  operationId: get_intelligence_brief__api_version__organizations__organization_id__intelligence_brief_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/organizations/{organization_id}/signals\n  method: get\n  operationId: get_organization_signals__api_version__organizations__organization_id__signals_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/people\n  method: post\n  operationId: enrich_people_unified__api_version__people_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/projects/lookup\n  method: post\n  operationId: lookup_projects__api_version__projects_lookup_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/signals\n  method: post\n  operationId: search_signals__api_version__signals_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v9/signals/priority\n  method: post\n  operationId: search_priority_signals__api_version__signals_priority_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/signals/priority/{item_id}/relevance\n  method: put\n  operationId: update_priority_signal_relevance__api_version__signals_priority__item_id__relevance_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/support/data-quality\n  method: post\n  operationId: create_data_quality_report__api_version__support_data_quality_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/support\n  method: post\n  operationId: create_support_request__api_version__support_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/teams\n  method: post\n  operationId: find_teams__api_version__teams_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/technologies/find\n  method: post\n  operationId: get_technologies__api_version__technologies_find_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v9/technologies/lookup\n  method: post\n  operationId: lookup_technologies__api_version__technologies_lookup_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v9/technologies/categories/lookup\n  method: post\n  operationId: lookup_technology_categories__api_version__technologies_categories_lookup_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/agentic-access/sumble-agentic-access.yml
summary_line: 26 operations · 12 acting
tags:
- Company
- Account Intelligence
- Sales Intelligence
- Data Enrichment
- Go-To-Market
- Technographics
- People Data
- Job Posts
- Signals
- MCP
---
