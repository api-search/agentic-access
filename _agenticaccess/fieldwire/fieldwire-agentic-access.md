---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 35
api_specs:
- filename: fieldwire-account-api-openapi.yml
  format: yaml
  label: Fieldwire Account API
  slug: fieldwire-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-account-api-openapi.yml
- filename: fieldwire-projects-api-openapi.yml
  format: yaml
  label: Fieldwire Projects API
  slug: fieldwire-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-projects-api-openapi.yml
- filename: fieldwire-tasks-api-openapi.yml
  format: yaml
  label: Fieldwire Tasks API
  slug: fieldwire-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-tasks-api-openapi.yml
- filename: fieldwire-plans-api-openapi.yml
  format: yaml
  label: Fieldwire Plans and Sheets API
  slug: fieldwire-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-plans-api-openapi.yml
- filename: fieldwire-forms-api-openapi.yml
  format: yaml
  label: Fieldwire Forms API
  slug: fieldwire-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-forms-api-openapi.yml
- filename: fieldwire-attachments-api-openapi.yml
  format: yaml
  label: Fieldwire Attachments and Media API
  slug: fieldwire-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-attachments-api-openapi.yml
- filename: fieldwire-financials-api-openapi.yml
  format: yaml
  label: Fieldwire Project Financials API
  slug: fieldwire-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-financials-api-openapi.yml
- filename: fieldwire-rfis-submittals-api-openapi.yml
  format: yaml
  label: Fieldwire RFIs and Submittals API
  slug: fieldwire-rfis-submittals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-rfis-submittals-api-openapi.yml
- filename: fieldwire-webhooks-api-openapi.yml
  format: yaml
  label: Fieldwire Webhooks API
  slug: fieldwire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 35
  write: 32
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{project_id}/transfer
operation_count: 69
overview: 'Fieldwire exposes 69 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 32 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fieldwire
provider_slug: fieldwire
slug: fieldwire-agentic-access
source_filename: fieldwire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fieldwire-account-api-openapi.yml, openapi/fieldwire-attachments-api-openapi.yml,\n  openapi/fieldwire-financials-api-openapi.yml, openapi/fieldwire-forms-api-openapi.yml, openapi/fieldwire-plans-api-openapi.yml,\n  openapi/fieldwire-projects-api-openapi.yml, openapi/fieldwire-rfis-submittals-api-openapi.yml,\n  openapi/fieldwire-tasks-api-openapi.yml, openapi/fieldwire-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    acting: 34\n    connected: 35\n  by_consequence:\n    write: 32\n    read: 35\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api_keys/jwt\n  method: post\n  operationId: getApiKeyJwt\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/users\n  method: get\n  operationId: getAccountUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/users/{user_id}\n  method: get\n  operationId: getAccountUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/users/{user_id}\n  method: patch\n  operationId: updateAccountUserById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates\n  method: get\n  operationId: getAccountFormTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates\n  method: post\n  operationId: createAccountFormTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates/{form_template_id}\n  method: get\n  operationId: getAccountFormTemplateById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}\n  method: patch\n\
  \  operationId: updateAccountFormTemplateById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/custom_stamps\n  method: get\n  operationId: getAccountCustomStamps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/custom_stamps\n  method: post\n  operationId: createAccountCustomStamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/aws_post_tokens\n  method: post\n  operationId:\
  \ addAwsPostTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/attachments\n  method: get\n  operationId: getAttachmentsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/attachments\n  method: post\n  operationId: createAttachmentInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/attachment_markups\n  method: get\n  operationId:\
  \ getAttachmentMarkupsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/attachment_markups\n  method: post\n  operationId: createAttachmentMarkupInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/budget_line_items\n  method: get\n  operationId: getBudgetLineItemsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/budget_line_items\n  method: post\n  operationId: createBudgetLineItemInProject\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/actual_costs\n  method: get\n  operationId: getActualCostsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/actual_costs\n  method: post\n  operationId: createActualCostInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/change_orders\n  method: get\n  operationId: getChangeOrdersInProject\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/change_orders\n  method: post\n  operationId: createChangeOrderInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates/{form_template_id}/sections\n  method: get\n  operationId: getFormTemplateSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}/sections\n  method: post\n  operationId: createFormTemplateSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/form_templates/{form_template_id}/sections/{section_id}/inputs\n  method: get\n  operationId: getFormTemplateSectionInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/form_templates/{form_template_id}/sections/{section_id}/inputs\n  method: post\n  operationId: createFormTemplateSectionInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/forms\n  method: get\n  operationId: getFormsInProject\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/forms\n  method: post\n  operationId: createFormInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/forms/{form_id}\n  method: get\n  operationId: getFormById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/floorplans\n  method: get\n  operationId: getFloorplansInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/floorplans\n\
  \  method: post\n  operationId: createFloorplanInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/floorplans/{floorplan_id}\n  method: get\n  operationId: getFloorplanById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/floorplans/{floorplan_id}\n  method: patch\n  operationId: updateFloorplanById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/sheets\n\
  \  method: get\n  operationId: getSheetsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/sheets\n  method: post\n  operationId: createSheetInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/hyperlinks\n  method: get\n  operationId: getHyperlinksInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/building_information_models\n  method: get\n  operationId: getBuildingInformationModelsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: get\n  operationId: getProjectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: patch\n  operationId: updateProjectById\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: deleteProjectById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/restore\n  method: post\n  operationId: restoreProjectById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/transfer\n  method: post\n\
  \  operationId: transferProject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/users\n  method: get\n  operationId: getProjectUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/users\n  method: post\n  operationId: createProjectUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/teams\n\
  \  method: get\n  operationId: getProjectTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/stats\n  method: get\n  operationId: getProjectStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/rfis\n  method: get\n  operationId: getRfisInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/rfis\n  method: post\n  operationId: createRfiInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /projects/{project_id}/rfis/{rfi_id}\n  method: get\n  operationId: getRfiById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/rfis/{rfi_id}\n  method: patch\n  operationId: updateRfiById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/submittals\n  method: get\n  operationId: getSubmittalsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/submittals\n  method: post\n  operationId: createSubmittalInProject\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/spec_sections\n  method: get\n  operationId: getSpecSectionsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/tasks\n  method: get\n  operationId: getTasksInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/tasks\n  method: post\n  operationId: createTaskInProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/tasks/{task_id}\n  method: get\n  operationId: getTaskById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/tasks/{task_id}\n  method: patch\n  operationId: updateTaskById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/tasks/{task_id}\n  method: delete\n  operationId: deleteTaskById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/tasks/{task_id}/check_items\n  method: get\n  operationId: getCheckItemsInTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/tasks/{task_id}/check_items\n  method: post\n  operationId: createCheckItemInTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/tasks/{task_id}/bubbles\n  method: get\n  operationId: getBubblesInTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/tasks/{task_id}/bubbles\n\
  \  method: post\n  operationId: createBubbleInTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/task_relations\n  method: get\n  operationId: getTaskRelationsInProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: getSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscription_id}\n  method: get\n  operationId: getSubscriptionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscription_id}\n  method: patch\n  operationId: updateSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscription_id}\n  method: delete\n  operationId: deleteSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/agentic-access/fieldwire-agentic-access.yml
summary_line: 69 operations · 34 acting
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
- Inspections
- Project Management
- Hilti
---
