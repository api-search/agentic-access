---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 17
api_specs:
- filename: fatsecret-exercise-diary-api-openapi.yml
  format: yaml
  label: fatsecret Exercise Diary API
  slug: fatsecret-exercise-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-exercise-diary-api-openapi.yml
- filename: fatsecret-food-diary-api-openapi.yml
  format: yaml
  label: fatsecret Food Diary API
  slug: fatsecret-food-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-food-diary-api-openapi.yml
- filename: fatsecret-foods-api-openapi.yml
  format: yaml
  label: fatsecret Foods API
  slug: fatsecret-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-foods-api-openapi.yml
- filename: fatsecret-image-recognition-api-openapi.yml
  format: yaml
  label: fatsecret Image Recognition API
  slug: fatsecret-image-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-image-recognition-api-openapi.yml
- filename: fatsecret-natural-language-processing-api-openapi.yml
  format: yaml
  label: fatsecret Natural Language Processing API
  slug: fatsecret-natural-language-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-natural-language-processing-api-openapi.yml
- filename: fatsecret-profile-foods-api-openapi.yml
  format: yaml
  label: fatsecret Profile Foods API
  slug: fatsecret-profile-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-foods-api-openapi.yml
- filename: fatsecret-profile-meals-api-openapi.yml
  format: yaml
  label: fatsecret Profile Meals API
  slug: fatsecret-profile-meals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-meals-api-openapi.yml
- filename: fatsecret-recipes-api-openapi.yml
  format: yaml
  label: fatsecret Recipes API
  slug: fatsecret-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-recipes-api-openapi.yml
- filename: fatsecret-reference-api-openapi.yml
  format: yaml
  label: fatsecret Reference API
  slug: fatsecret-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-reference-api-openapi.yml
- filename: fatsecret-weight-tracking-api-openapi.yml
  format: yaml
  label: fatsecret Weight Tracking API
  slug: fatsecret-weight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-weight-tracking-api-openapi.yml
consequence_counts:
  read: 17
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fatsecret Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'fatsecret exposes 23 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fatsecret
provider_slug: fatsecret
slug: fatsecret-agentic-access
source_filename: fatsecret-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fatsecret-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 17\n    acting: 6\n  by_consequence:\n    read: 17\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /foods/search/v5\n  method: get\n  operationId: searchFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/autocomplete/v2\n  method: get\n  operationId: autocompleteFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/barcode/find-by-id/v1\n\
  \  method: get\n  operationId: findFoodByBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/v4\n  method: get\n  operationId: getFood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-brands/v2\n  method: get\n  operationId: listFoodBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-categories/v2\n  method: get\n  operationId: listFoodCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-sub-categories/v2\n  method: get\n  operationId: listFoodSubCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipes/search/v3\n  method: get\n  operationId: searchRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipe/v2\n  method: get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipe-types/v2\n  method: get\n  operationId: listRecipeTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exercises/v2\n  method: get\n  operationId: listExercises\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/favorites/v2\n  method: get\n  operationId: getFavoriteFoods\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/favorite/add/v2\n  method: post\n  operationId: addFavoriteFood\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food/favorite/delete/v2\n  method: post\n  operationId: deleteFavoriteFood\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-entries/v2\n  method: get\n  operationId: getFoodEntries\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-entries/v2\n  method: post\n  operationId: createFoodEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-entries/month/v2\n  method: get\n  operationId: getFoodEntriesMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exercise-entries/v2\n  method: get\n  operationId: getExerciseEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exercise-entries/v2\n  method: post\n  operationId: commitExerciseEntries\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /weights/v2\n  method: get\n  operationId: getWeights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weights/v2\n  method: post\n  operationId: updateWeight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saved-meals/v2\n  method: get\n  operationId: listSavedMeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /saved-meals/v2\n  method: post\n  operationId: createSavedMeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/agentic-access/fatsecret-agentic-access.yml
summary_line: 23 operations · 6 acting
tags:
- Artificial Intelligence
- Barcode Scanning
- Calories
- Diets
- Image Recognition
- Natural Language Processing
- Exercise
- Fitness
- Food Diary
- Health
- Macronutrients
- Nutrition
- Recipes
- Weight Tracking
---
