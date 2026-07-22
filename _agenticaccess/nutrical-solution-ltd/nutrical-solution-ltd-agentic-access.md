---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: nutrical-solution-ltd-openapi.yml
  format: yaml
  label: NutriCal Food & Nutrition API
  slug: nutrical-food-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-openapi.yml
consequence_counts:
  read: 12
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nutrical Solution Ltd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Nutrical Solution Ltd exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nutrical Solution Ltd
provider_slug: nutrical-solution-ltd
slug: nutrical-solution-ltd-agentic-access
source_filename: nutrical-solution-ltd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/nutrical-solution-ltd-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 9\n    connected: 12\n  by_consequence:\n    write: 9\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /entity/create\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/ingredients/\n  method: get\n  operationId: listIngredients\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/recipe-categories/\n  method: get\n  operationId: listRecipeCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/recipe-categories/\n  method: post\n  operationId: addRecipeCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/recipe-categories/{recipeCategoryId}\n  method: post\n  operationId: updateRecipeCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/recipe-sub-categories/\n  method: get\n  operationId: listRecipeSubCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/recipes/\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/recipes/\n  method: post\n  operationId: createRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/recipes/{recipeId}/\n  method:\
  \ get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/recipes/{recipeId}\n  method: patch\n  operationId: updateRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/recipes/{recipeId}\n  method: delete\n  operationId: deleteRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/meal-plans/\n  method: get\n  operationId: listMealPlans\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/meal-plans/{mealPlanId}/\n  method: get\n  operationId: getMealPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/meal-plan-customers/\n  method: get\n  operationId: listMealPlanCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/meal-plan-customers/\n  method: post\n  operationId: createMealPlanCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /external/api/v2/meal-plan-customers/{mealplanCustomerId}/\n  method: get\n  operationId: getMealPlanCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v2/meal-plan-customers/{mealplanCustomerId}/\n  method: patch\n  operationId: updateMealPlanCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v2/meal-plan-customers/{mealplanCustomerId}/\n  method: delete\n  operationId: deleteMealPlanCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/api/v1/nutrients/\n  method: get\n  operationId: listNutrients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/api/v1/allergens/\n  method: get\n  operationId: listAllergens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/api/v1/may-contain-allergens/\n  method: get\n  operationId: listMayContainAllergens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/agentic-access/nutrical-solution-ltd-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Company
- Food
- Nutrition
- Health
- Recipes
- Meal Plans
- Food Labeling
- Compliance
- Restaurants
- GCC
---
