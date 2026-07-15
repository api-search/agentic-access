---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 34
api_specs:
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Athlete API
  slug: trainingpeaks-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workouts API
  slug: trainingpeaks-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workout Details API
  slug: trainingpeaks-workout-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workout of the Day API
  slug: trainingpeaks-workout-of-the-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Metrics API
  slug: trainingpeaks-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Nutrition API
  slug: trainingpeaks-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Coach API
  slug: trainingpeaks-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks File Upload API
  slug: trainingpeaks-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Events and Routes API
  slug: trainingpeaks-events-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Webhooks API
  slug: trainingpeaks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
consequence_counts:
  read: 34
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trainingpeaks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 49
overview: 'TrainingPeaks exposes 49 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TrainingPeaks
provider_slug: trainingpeaks
slug: trainingpeaks-agentic-access
source_filename: trainingpeaks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/trainingpeaks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 34\n    acting: 15\n  by_consequence:\n    read: 34\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/info/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/athlete/profile\n  method: get\n  operationId: getAthleteProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/athlete/zones\n\
  \  method: get\n  operationId: getAthleteZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/athlete/zones/{zoneType}\n  method: get\n  operationId: getAthleteZonesByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/profile\n  method: get\n  operationId: getCoachProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/athletes\n  method: get\n  operationId: getCoachAthletes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/athletes/zones\n  method: get\n  operationId: getCoachAthleteZones\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/athletes/zones/{zoneType}\n  method: get\n  operationId: getCoachAthleteZonesByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/assistants\n  method: get\n  operationId: getCoachAssistants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/assistants/{assistantId}\n  method: get\n  operationId: getCoachAssistant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coach/assistants/{assistantId}/athletes\n  method: get\n  operationId: getCoachAssistantAthletes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/file\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/metrics/{metricId}\n  method: get\n  operationId: getMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/metrics/{startDate}/{endDate}\n  method: get\n  operationId: getMetricsByDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/metrics/{athleteId}/{startDate}/{endDate}\n  method: get\n  operationId: getAthleteMetrics\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/metrics\n  method: post\n  operationId: createMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/athletes/{athleteId}/nutrition\n  method: get\n  operationId: getNutrition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/athletes/{athleteId}/nutrition\n  method: post\n  operationId: createNutrition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/athletes/{athleteId}/nutrition/{nutritionId}\n  method: put\n  operationId: updateNutrition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/athletes/{athleteId}/nutrition/{nutritionId}\n  method: delete\n  operationId: deleteNutrition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workouts/{startDate}/{endDate}\n  method: get\n  operationId: getWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/{startDate}/{endDate}\n  method: get\n  operationId: getAthleteWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/changed\n  method: get\n  operationId: getChangedWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/changed\n  method: get\n  operationId: getChangedWorkoutsForAthlete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/wod/{date}\n  method: get\n  operationId: getWorkoutOfTheDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/workouts/wod/file/{workoutId}/\n  method: get\n  operationId: getWorkoutOfTheDayFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/plan\n  method: post\n  operationId: createWorkout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workouts/plan/{id}\n  method: put\n  operationId: updateWorkout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workouts/id/{id}\n  method: get\n\
  \  operationId: getWorkoutById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/id/{id}\n  method: delete\n  operationId: deleteWorkoutById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workouts/{athleteId}/id/{id}\n  method: get\n  operationId: getAthleteWorkoutById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/id/{id}\n  method: delete\n  operationId: deleteAthleteWorkoutById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workouts/id/{id}/meanmaxes\n  method: get\n  operationId: getWorkoutMeanMax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/id/{id}/meanmaxes\n  method: get\n  operationId: getAthleteWorkoutMeanMax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/id/{id}/timeinzones\n  method: get\n  operationId: getWorkoutTimeInZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/id/{id}/timeinzones\n  method: get\n  operationId: getAthleteWorkoutTimeInZones\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/id/{id}/details\n  method: get\n  operationId: getWorkoutDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/id/{id}/details\n  method: get\n  operationId: getAthleteWorkoutDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workouts/{athleteId}/id/{workoutId}/comment\n  method: post\n  operationId: createWorkoutComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v2/athletes/{athleteId}/strength-workouts\n  method: get\n  operationId: getStrengthWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events/next\n  method: get\n  operationId: getNextEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events/{date}\n  method: get\n  operationId: getEventsByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events\n  method: post\n  operationId: createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/athletes/{athleteId}/routes\n  method: get\n  operationId: getRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/athlete/{athleteId}/routes\n  method: post\n  operationId: createRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/subscriptions\n  method: get\n  operationId: getWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/subscriptions/{subscriptionId}\n  method: put\n  operationId: updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/agentic-access/trainingpeaks-agentic-access.yml
summary_line: 49 operations · 15 acting
tags:
- Fitness
- Endurance Training
- Workouts
- Coaching
- Sports
- Health
- Wearables
---
