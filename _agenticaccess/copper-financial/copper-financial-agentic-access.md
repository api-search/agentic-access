---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: copper-financial-account-api-openapi.yml
  format: yaml
  label: Copper Financial Account API
  slug: copper-financial-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-account-api-openapi.yml
- filename: copper-financial-activities-api-openapi.yml
  format: yaml
  label: Copper Financial Activities API
  slug: copper-financial-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-activities-api-openapi.yml
- filename: copper-financial-companies-api-openapi.yml
  format: yaml
  label: Copper Financial Companies API
  slug: copper-financial-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-companies-api-openapi.yml
- filename: copper-financial-custom-fields-api-openapi.yml
  format: yaml
  label: Copper Financial Custom Fields API
  slug: copper-financial-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-custom-fields-api-openapi.yml
- filename: copper-financial-field-layouts-api-openapi.yml
  format: yaml
  label: Copper Financial Field Layouts API
  slug: copper-financial-field-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-field-layouts-api-openapi.yml
- filename: copper-financial-leads-api-openapi.yml
  format: yaml
  label: Copper Financial Leads API
  slug: copper-financial-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-leads-api-openapi.yml
- filename: copper-financial-opportunities-api-openapi.yml
  format: yaml
  label: Copper Financial Opportunities API
  slug: copper-financial-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-opportunities-api-openapi.yml
- filename: copper-financial-people-api-openapi.yml
  format: yaml
  label: Copper Financial People API
  slug: copper-financial-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-people-api-openapi.yml
- filename: copper-financial-related-items-api-openapi.yml
  format: yaml
  label: Copper Financial Related Items API
  slug: copper-financial-related-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-related-items-api-openapi.yml
- filename: copper-financial-tags-api-openapi.yml
  format: yaml
  label: Copper Financial Tags API
  slug: copper-financial-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-tags-api-openapi.yml
- filename: copper-financial-tasks-api-openapi.yml
  format: yaml
  label: Copper Financial Tasks API
  slug: copper-financial-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-tasks-api-openapi.yml
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Copper Financial Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Copper Financial exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Copper Financial
provider_slug: copper-financial
slug: copper-financial-agentic-access
source_filename: copper-financial-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: generated\nsource: openapi/copper-financial-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /users/search\n  method: post\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/search\n  method: post\n  operationId: searchLeads\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{id}/activities\n  method: post\n  operationId: getLeadActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_sources\n  method: get\n  operationId: listCustomerSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lead_statuses\n  method: get\n  operationId: listLeadStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/search\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /people/fetch_by_email\n  method: post\n  operationId: getPersonByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{id}/activities\n  method: post\n  operationId: getPersonActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact_types\n  method: get\n  operationId: listContactTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/search\n  method: post\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{id}/activities\n  method: post\n  operationId: getCompanyActivities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}\n  method: get\n  operationId: getOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/activities\n  method: post\n  operationId: getOpportunityActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/search\n  method: post\n  operationId: searchOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loss_reasons\n  method: get\n  operationId: listLossReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipeline_stages\n  method: get\n  operationId: listPipelineStages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/search\n  method: post\n  operationId: searchTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities/search\n  method: post\n  operationId: searchActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity_types\n  method: get\n  operationId: listActivityTypes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_activity_types\n  method: get\n  operationId: listCustomActivityTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_field_definitions\n  method: get\n  operationId: listCustomFieldDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field_layouts/by_entity/{entity_type}\n  method: get\n  operationId: listFieldLayoutByEntityType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entity_type}/{entity_id}/related\n  method: get\n  operationId: getRelatedItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entity_type}/{entity_id}/related/{related_entity_type}\n  method: get\n  operationId: getRelatedItemsByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/agentic-access/copper-financial-agentic-access.yml
summary_line: 27 operations
tags:
- Company
- CRM
- Software-as-a-Service
- Sales
- Marketing
---
