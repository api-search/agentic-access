---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: djangocms-rest-openapi.yml
  format: yaml
  label: djangocms-rest API
  slug: djangocms-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/django-cms/main/openapi/djangocms-rest-openapi.yml
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Django Cms Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Django CMS exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Django CMS
provider_slug: django-cms
slug: django-cms-agentic-access
source_filename: django-cms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/djangocms-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /healthcheck/\n  method: get\n  operationId: healthcheck_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /languages/\n  method: get\n  operationId: language_list_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/pages-tree/\n  method: get\n  operationId:\
  \ page_tree_list_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/pages-list/\n  method: get\n  operationId: page_list_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/pages/\n  method: get\n  operationId: page_root_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/pages/{path}/\n  method: get\n  operationId: page_detail_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/page_search/\n  method: get\n  operationId: page_search_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/placeholders/{content_type_id}/{object_id}/{slot}/\n  method: get\n  operationId: placeholder_detail_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugins/\n  method: get\n  operationId: plugin_list_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/menu/\n  method: get\n  operationId: menu_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/menu/{from_level}/{to_level}/{extra_inactive}/{extra_active}/\n  method: get\n  operationId: menu_levels_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/menu/{from_level}/{to_level}/{extra_inactive}/{extra_active}/{path}/\n  method: get\n  operationId: menu_levels_path_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/menu/{root_id}/{from_level}/{to_level}/{extra_inactive}/{extra_active}/\n  method: get\n  operationId: menu_root_levels_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/menu/{root_id}/{from_level}/{to_level}/{extra_inactive}/{extra_active}/{path}/\n  method: get\n  operationId: menu_root_levels_path_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/submenu/{levels}/{root_level}/{nephews}/\n\
  \  method: get\n  operationId: submenu_levels_root_nephews_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/submenu/{levels}/{root_level}/{nephews}/{path}/\n  method: get\n  operationId: submenu_levels_root_nephews_path_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/submenu/{levels}/{root_level}/\n  method: get\n  operationId: submenu_levels_root_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/submenu/{levels}/\n  method: get\n  operationId: submenu_levels_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /{language}/submenu/\n  method: get\n  operationId: submenu_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/breadcrumbs/\n  method: get\n  operationId: breadcrumbs_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/breadcrumbs/{path}/\n  method: get\n  operationId: breadcrumbs_path_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/breadcrumbs/{start_level}/\n  method: get\n  operationId: breadcrumbs_level_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{language}/breadcrumbs/{start_level}/{path}/\n\
  \  method: get\n  operationId: breadcrumbs_level_path_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/django-cms/refs/heads/main/agentic-access/django-cms-agentic-access.yml
summary_line: 23 operations
tags:
- CMS
- Content Management
- Django
- Python
- Headless CMS
- REST API
- Open Source
- Pages
- Plugins
- Placeholders
---
