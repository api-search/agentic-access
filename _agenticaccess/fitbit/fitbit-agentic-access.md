---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 37
api_specs:
- filename: fitbit-activity-api-openapi.yml
  format: yaml
  label: Fitbit Activity API
  slug: fitbit-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-activity-api-openapi.yml
- filename: fitbit-heart-rate-api-openapi.yml
  format: yaml
  label: Fitbit Heart Rate API
  slug: fitbit-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-heart-rate-api-openapi.yml
- filename: fitbit-sleep-api-openapi.yml
  format: yaml
  label: Fitbit Sleep API
  slug: fitbit-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-sleep-api-openapi.yml
- filename: fitbit-body-api-openapi.yml
  format: yaml
  label: Fitbit Body API
  slug: fitbit-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-body-api-openapi.yml
- filename: fitbit-nutrition-api-openapi.yml
  format: yaml
  label: Fitbit Nutrition API
  slug: fitbit-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-nutrition-api-openapi.yml
- filename: fitbit-user-api-openapi.yml
  format: yaml
  label: Fitbit User API
  slug: fitbit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-user-api-openapi.yml
- filename: fitbit-devices-api-openapi.yml
  format: yaml
  label: Fitbit Devices API
  slug: fitbit-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-devices-api-openapi.yml
- filename: fitbit-subscriptions-api-openapi.yml
  format: yaml
  label: Fitbit Subscriptions API
  slug: fitbit-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-subscriptions-api-openapi.yml
- filename: fitbit-friends-api-openapi.yml
  format: yaml
  label: Fitbit Friends API
  slug: fitbit-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-friends-api-openapi.yml
- filename: fitbit-spo2-breathing-temperature-api-openapi.yml
  format: yaml
  label: Fitbit SpO2, Breathing Rate, Temperature, HRV, and Cardio Fitness API
  slug: fitbit-spo2-breathing-temperature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-spo2-breathing-temperature-api-openapi.yml
- filename: fitbit-ecg-irn-api-openapi.yml
  format: yaml
  label: Fitbit ECG and Irregular Rhythm Notifications API
  slug: fitbit-ecg-irn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-ecg-irn-api-openapi.yml
- filename: fitbit-authorization-api-openapi.yml
  format: yaml
  label: Fitbit Authorization API
  slug: fitbit-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-authorization-api-openapi.yml
consequence_counts:
  read: 37
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Fitbit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/revoke
operation_count: 55
overview: 'Fitbit exposes 55 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fitbit
provider_slug: fitbit
slug: fitbit-agentic-access
source_filename: fitbit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fitbit-activity-api-openapi.yml, openapi/fitbit-authorization-api-openapi.yml,\n  openapi/fitbit-body-api-openapi.yml, openapi/fitbit-devices-api-openapi.yml, openapi/fitbit-ecg-irn-api-openapi.yml,\n  openapi/fitbit-friends-api-openapi.yml, openapi/fitbit-heart-rate-api-openapi.yml, openapi/fitbit-nutrition-api-openapi.yml,\n  openapi/fitbit-sleep-api-openapi.yml, openapi/fitbit-spo2-breathing-temperature-api-openapi.yml,\n  openapi/fitbit-subscriptions-api-openapi.yml, openapi/fitbit-user-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 37\n    acting: 18\n  by_consequence:\n    read: 37\n    write: 17\n    safety-critical: 1\n\
  \  human_in_the_loop_required: 1\noperations:\n- path: /1/user/{user-id}/activities/date/{date}.json\n  method: get\n  operationId: getDailyActivitySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - activity\n- path: /1/user/{user-id}/activities.json\n  method: post\n  operationId: logActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - activity\n- path: /1/user/{user-id}/activities/{activity-log-id}.json\n  method: delete\n  operationId: deleteActivityLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - activity\n- path: /1/user/{user-id}/activities/list.json\n  method: get\n  operationId: getActivityLogList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - activity\n- path: /1/user/{user-id}/activities/goals/{period}.json\n  method: get\n  operationId: getActivityGoals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - activity\n- path: /1/user/{user-id}/activities/active-zone-minutes/date/{date}/{period}.json\n  method: get\n  operationId: getAzmTimeSeriesByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - activity\n\
  - path: /1/user/{user-id}/activities/steps/date/{base-date}/{end-date}.json\n  method: get\n  operationId: getActivityTimeSeriesByDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - activity\n- path: /oauth2/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.1/oauth2/introspect\n  method: post\n  operationId: introspectToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /1/user/{user-id}/body/log/weight/date/{date}.json\n  method: get\n  operationId: getWeightLogsByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - weight\n- path: /1/user/{user-id}/body/log/weight/date/{date}.json\n  method: post\n  operationId: logWeight\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - weight\n- path: /1/user/{user-id}/body/log/weight/{weight-log-id}.json\n  method: delete\n  operationId: deleteWeightLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - weight\n- path: /1/user/{user-id}/body/log/fat/date/{date}.json\n  method: get\n  operationId: getBodyFatLogsByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - weight\n\
  - path: /1/user/{user-id}/body/{resource-path}/date/{date}/{period}.json\n  method: get\n  operationId: getBodyTimeSeriesByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - weight\n- path: /1/user/{user-id}/body/log/weight/goal.json\n  method: get\n  operationId: getBodyWeightGoal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - weight\n- path: /1/user/{user-id}/devices.json\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - settings\n- path: /1/user/{user-id}/devices/tracker/{tracker-id}/alarms.json\n  method: get\n  operationId: getAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - settings\n- path: /1/user/{user-id}/devices/tracker/{tracker-id}/alarms.json\n  method: post\n  operationId: addAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - settings\n- path: /1/user/{user-id}/devices/tracker/{tracker-id}/alarms/{alarm-id}.json\n  method: delete\n  operationId: deleteAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - settings\n- path: /1/user/{user-id}/ecg/list.json\n  method:\
  \ get\n  operationId: getEcgLogList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - electrocardiogram\n    - irregular_rhythm_notifications\n- path: /1/user/{user-id}/irn/alerts/list.json\n  method: get\n  operationId: getIrnAlertsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - electrocardiogram\n    - irregular_rhythm_notifications\n- path: /1/user/{user-id}/irn/profile.json\n  method: get\n  operationId: getIrnProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - electrocardiogram\n    - irregular_rhythm_notifications\n- path: /1.1/user/{user-id}/friends.json\n  method: get\n  operationId: getFriends\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - social\n- path: /1.1/user/{user-id}/leaderboard/friends.json\n  method: get\n  operationId: getFriendsLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - social\n- path: /1/user/{user-id}/activities/heart/date/{date}/{period}.json\n  method: get\n  operationId: getHeartRateTimeSeriesByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - heartrate\n- path: /1/user/{user-id}/activities/heart/date/{base-date}/{end-date}.json\n  method: get\n  operationId: getHeartRateTimeSeriesByDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - heartrate\n- path: /1/user/{user-id}/activities/heart/date/{date}/1d/{detail-level}.json\n  method: get\n  operationId: getHeartRateIntradayTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - heartrate\n- path: /1/user/{user-id}/foods/log/date/{date}.json\n  method: get\n  operationId: getFoodLogsByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - nutrition\n- path: /1/user/{user-id}/foods/log.json\n  method: post\n  operationId: logFood\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - nutrition\n- path: /1/user/{user-id}/foods/log/{food-log-id}.json\n  method: delete\n  operationId: deleteFoodLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - nutrition\n- path: /1/user/{user-id}/foods/log/water/date/{date}.json\n  method: get\n  operationId: getWaterLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - nutrition\n- path: /1/user/{user-id}/foods/log/water.json\n  method: post\n  operationId: logWater\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - nutrition\n- path: /1/foods/search.json\n  method: get\n  operationId: searchFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - nutrition\n- path: /1/user/{user-id}/foods/log/goal.json\n  method: get\n  operationId: getFoodGoals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - nutrition\n- path: /1.2/user/{user-id}/sleep/date/{date}.json\n  method: get\n  operationId: getSleepLogByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - sleep\n- path: /1.2/user/{user-id}/sleep/date/{base-date}/{end-date}.json\n  method: get\n  operationId: getSleepLogByDateRange\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - sleep\n- path: /1.2/user/{user-id}/sleep/list.json\n  method: get\n  operationId: getSleepLogList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - sleep\n- path: /1.2/user/{user-id}/sleep.json\n  method: post\n  operationId: logSleep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - sleep\n- path: /1.2/user/{user-id}/sleep/{log-id}.json\n  method: delete\n  operationId: deleteSleepLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - sleep\n- path: /1/user/{user-id}/sleep/goal.json\n  method: get\n  operationId: getSleepGoal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - sleep\n- path: /1/user/{user-id}/sleep/goal.json\n  method: post\n  operationId: updateSleepGoal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - sleep\n- path: /1/user/{user-id}/spo2/date/{date}.json\n  method: get\n  operationId: getSpo2SummaryByDate\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/spo2/date/{base-date}/{end-date}.json\n  method: get\n  operationId: getSpo2SummaryByDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/br/date/{date}.json\n  method: get\n  operationId: getBreathingRateByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/temp/skin/date/{date}.json\n\
  \  method: get\n  operationId: getSkinTemperatureByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/temp/core/date/{date}.json\n  method: get\n  operationId: getCoreTemperatureByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/hrv/date/{date}.json\n  method: get\n  operationId: getHrvByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n\
  \    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/cardioscore/date/{date}.json\n  method: get\n  operationId: getVo2MaxByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cardio_fitness\n    - heartrate\n    - oxygen_saturation\n    - respiratory_rate\n    - temperature\n- path: /1/user/{user-id}/{collection-path}/apiSubscriptions/{subscription-id}.json\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/user/{user-id}/{collection-path}/apiSubscriptions/{subscription-id}.json\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/user/{user-id}/{collection-path}/apiSubscriptions.json\n  method: get\n  operationId: getSubscriptionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/user/{user-id}/profile.json\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - profile\n- path: /1/user/{user-id}/profile.json\n  method: post\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/agentic-access/fitbit-agentic-access.yml
summary_line: 55 operations · 18 acting · 1 human-in-the-loop
tags:
- Wearable
- Health
- Fitness
- Activity Tracking
- Heart Rate
- Sleep
- Google
- IoT
---
