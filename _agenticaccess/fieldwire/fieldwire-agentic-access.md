---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 24
api_specs:
- filename: fieldwire-actual-costs-api-openapi.yml
  format: yaml
  label: Fieldwire Actual Costs API
  slug: fieldwire-actual-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-actual-costs-api-openapi.yml
- filename: fieldwire-authentication-api-openapi.yml
  format: yaml
  label: Fieldwire Authentication API
  slug: fieldwire-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-authentication-api-openapi.yml
- filename: fieldwire-budget-line-items-api-openapi.yml
  format: yaml
  label: Fieldwire Budget Line Items API
  slug: fieldwire-budget-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-budget-line-items-api-openapi.yml
- filename: fieldwire-building-information-models-api-openapi.yml
  format: yaml
  label: Fieldwire Building Information Models API
  slug: fieldwire-building-information-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-building-information-models-api-openapi.yml
- filename: fieldwire-change-orders-api-openapi.yml
  format: yaml
  label: Fieldwire Change Orders API
  slug: fieldwire-change-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-change-orders-api-openapi.yml
- filename: fieldwire-custom-stamps-api-openapi.yml
  format: yaml
  label: Fieldwire Custom Stamps API
  slug: fieldwire-custom-stamps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-custom-stamps-api-openapi.yml
- filename: fieldwire-form-inputs-api-openapi.yml
  format: yaml
  label: Fieldwire Form Inputs API
  slug: fieldwire-form-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-form-inputs-api-openapi.yml
- filename: fieldwire-form-records-api-openapi.yml
  format: yaml
  label: Fieldwire Form Records API
  slug: fieldwire-form-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-form-records-api-openapi.yml
- filename: fieldwire-form-sections-api-openapi.yml
  format: yaml
  label: Fieldwire Form Sections API
  slug: fieldwire-form-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-form-sections-api-openapi.yml
- filename: fieldwire-form-templates-api-openapi.yml
  format: yaml
  label: Fieldwire Form Templates API
  slug: fieldwire-form-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-form-templates-api-openapi.yml
- filename: fieldwire-hyperlinks-api-openapi.yml
  format: yaml
  label: Fieldwire Hyperlinks API
  slug: fieldwire-hyperlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-hyperlinks-api-openapi.yml
- filename: fieldwire-rfis-api-openapi.yml
  format: yaml
  label: Fieldwire RFIs API
  slug: fieldwire-rfis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-rfis-api-openapi.yml
- filename: fieldwire-sheets-api-openapi.yml
  format: yaml
  label: Fieldwire Sheets API
  slug: fieldwire-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-sheets-api-openapi.yml
- filename: fieldwire-spec-sections-api-openapi.yml
  format: yaml
  label: Fieldwire Spec Sections API
  slug: fieldwire-spec-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-spec-sections-api-openapi.yml
- filename: fieldwire-submittals-api-openapi.yml
  format: yaml
  label: Fieldwire Submittals API
  slug: fieldwire-submittals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-submittals-api-openapi.yml
- filename: fieldwire-subscriptions-api-openapi.yml
  format: yaml
  label: Fieldwire Subscriptions API
  slug: fieldwire-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-subscriptions-api-openapi.yml
- filename: fieldwire-users-api-openapi.yml
  format: yaml
  label: Fieldwire Users API
  slug: fieldwire-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-users-api-openapi.yml
- filename: fieldwire-floor-plans-api-openapi.yml
  format: yaml
  label: Fieldwire Floor Plans API
  slug: fieldwire-floor-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-floor-plans-api-openapi.yml
consequence_counts:
  physical: 1
  read: 24
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fieldwire Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{project_id}/change_orders
operation_count: 43
overview: 'Fieldwire exposes 43 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 18 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fieldwire
provider_slug: fieldwire
slug: fieldwire-agentic-access
source_filename: fieldwire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/fieldwire-actual-costs-api-openapi.yml, openapi/fieldwire-authentication-api-openapi.yml,\n  openapi/fieldwire-budget-line-items-api-openapi.yml, openapi/fieldwire-building-information-models-api-openapi.yml,\n  openapi/fieldwire-change-orders-api-openapi.yml, openapi/fieldwire-custom-stamps-api-openapi.yml,\n  openapi/fieldwire-floor-plans-api-openapi.yml, openapi/fieldwire-form-inputs-api-openapi.yml,\n  openapi/fieldwire-form-records-api-openapi.yml, openapi/fieldwire-form-sections-api-openapi.yml,\n  openapi/fieldwire-form-templates-api-openapi.yml, openapi/fieldwire-hyperlinks-api-openapi.yml,\n  openapi/fieldwire-rfis-api-openapi.yml, openapi/fieldwire-sheets-api-openapi.yml, openapi/fieldwire-spec-sections-api-openapi.yml,\n  openapi/fieldwire-submittals-api-openapi.yml, openapi/fieldwire-subscriptions-api-openapi.yml,\n  openapi/fieldwire-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution\
  \ contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 24\n    acting: 19\n  by_consequence:\n    read: 24\n    write: 18\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project_id}/actual_costs\n  method: get\n  operationId: getActualCostsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/actual_costs\n  method: post\n  operationId: createActualCostInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api_keys/jwt\n  method: post\n  operationId: getApiKeyJwt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/budget_line_items\n  method: get\n  operationId: getBudgetLineItemsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/budget_line_items\n  method: post\n  operationId: createBudgetLineItemInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/building_information_models\n  method: get\n  operationId: getBuildingInformationModelsInProject\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/change_orders\n  method: get\n  operationId: getChangeOrdersInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/change_orders\n  method: post\n  operationId: createChangeOrderInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/custom_stamps\n  method: get\n  operationId: getAccountCustomStamps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/custom_stamps\n  method: post\n  operationId: createAccountCustomStamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/floorplans\n  method: get\n  operationId: getFloorplansInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/floorplans\n  method: post\n  operationId: createFloorplanInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /projects/{project_id}/floorplans/{floorplan_id}\n  method: get\n  operationId: getFloorplanById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/floorplans/{floorplan_id}\n  method: patch\n  operationId: updateFloorplanById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates/{form_template_id}/sections/{section_id}/inputs\n  method: get\n  operationId: getFormTemplateSectionInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}/sections/{section_id}/inputs\n\
  \  method: post\n  operationId: createFormTemplateSectionInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/forms\n  method: get\n  operationId: getFormsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/forms\n  method: post\n  operationId: createFormInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/forms/{form_id}\n  method: get\n\
  \  operationId: getFormById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}/sections\n  method: get\n  operationId: getFormTemplateSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}/sections\n  method: post\n  operationId: createFormTemplateSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates\n  method: get\n  operationId: getAccountFormTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates\n  method: post\n  operationId: createAccountFormTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates/{form_template_id}\n  method: get\n  operationId: getAccountFormTemplateById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}\n  method: patch\n  operationId: updateAccountFormTemplateById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/hyperlinks\n  method: get\n  operationId: getHyperlinksInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/rfis\n  method: get\n  operationId: getRfisInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/rfis\n  method: post\n  operationId: createRfiInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/rfis/{rfi_id}\n  method: get\n  operationId: getRfiById\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/rfis/{rfi_id}\n  method: patch\n  operationId: updateRfiById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/sheets\n  method: get\n  operationId: getSheetsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/sheets\n  method: post\n  operationId: createSheetInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/spec_sections\n  method: get\n  operationId: getSpecSectionsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/submittals\n  method: get\n  operationId: getSubmittalsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/submittals\n  method: post\n  operationId: createSubmittalInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n\
  \  method: get\n  operationId: getSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscription_id}\n  method: get\n  operationId: getSubscriptionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscription_id}\n  method: patch\n  operationId: updateSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscription_id}\n  method: delete\n  operationId: deleteSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/users\n  method: get\n  operationId: getAccountUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/users/{user_id}\n  method: get\n  operationId: getAccountUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/users/{user_id}\n\
  \  method: patch\n  operationId: updateAccountUserById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/agentic-access/fieldwire-agentic-access.yml
summary_line: 43 operations · 19 acting
tags:
- Construction
- Construction Technology
- ConTech
- Field Management
- Punch List
- Plans
- Drawings
- BIM
- Forms
- Inspection
- Project Management
- Hilti
---
