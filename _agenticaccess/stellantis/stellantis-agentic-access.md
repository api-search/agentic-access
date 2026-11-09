---
acting_count: 107
action_class_counts:
  acting: 107
  connected: 122
api_specs:
- filename: stellantis-grouping-api-openapi.yml
  format: yaml
  label: Stellantis Grouping API
  slug: stellantis-grouping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-grouping-api-openapi.yml
- filename: stellantis-data-stream-api-openapi.yml
  format: yaml
  label: Stellantis Data Stream API
  slug: stellantis-data-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-data-stream-api-openapi.yml
- filename: stellantis-auth-api-openapi.yml
  format: yaml
  label: Stellantis Auth API
  slug: stellantis-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-auth-api-openapi.yml
- filename: stellantis-bugs-api-openapi.yml
  format: yaml
  label: Stellantis Bugs API
  slug: stellantis-bugs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-bugs-api-openapi.yml
- filename: stellantis-cloud-data-treatment-api-openapi.yml
  format: yaml
  label: Stellantis Vehicles API
  slug: stellantis-cloud-data-treatment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-data-treatment-api-openapi.yml
- filename: stellantis-cloud-docg-device-management-api-openapi.yml
  format: yaml
  label: Stellantis Cloud Docg Device Management API
  slug: stellantis-cloud-docg-device-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-docg-device-management-api-openapi.yml
- filename: stellantis-cloud-notification-center-api-openapi.yml
  format: yaml
  label: Stellantis Cloud Notification Center API
  slug: stellantis-cloud-notification-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-notification-center-api-openapi.yml
- filename: stellantis-connected-car-b2b-api-openapi.yml
  format: yaml
  label: Stellantis Capabilities API
  slug: stellantis-connected-car-b2b-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-connected-car-b2b-api-openapi.yml
- filename: stellantis-connected-car-b2c-api-openapi.yml
  format: yaml
  label: Stellantis Connected Car B2C API
  slug: stellantis-connected-car-b2c-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-connected-car-b2c-api-openapi.yml
- filename: stellantis-data-api-openapi.yml
  format: yaml
  label: Stellantis Data API
  slug: stellantis-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-data-api-openapi.yml
- filename: stellantis-feedback-api-openapi.yml
  format: yaml
  label: Stellantis Feedback API
  slug: stellantis-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-feedback-api-openapi.yml
- filename: stellantis-geofence-breaches-api-openapi.yml
  format: yaml
  label: Stellantis Geofence Breaches API
  slug: stellantis-geofence-breaches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofence-breaches-api-openapi.yml
- filename: stellantis-geofence-collection-api-openapi.yml
  format: yaml
  label: Stellantis Geofence Collection API
  slug: stellantis-geofence-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofence-collection-api-openapi.yml
- filename: stellantis-geofencing-notifications-api-openapi.yml
  format: yaml
  label: Stellantis Geofencing Notifications API
  slug: stellantis-geofencing-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofencing-notifications-api-openapi.yml
- filename: stellantis-hackathon-register-api-openapi.yml
  format: yaml
  label: Stellantis Hackathon Register API
  slug: stellantis-hackathon-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-hackathon-register-api-openapi.yml
- filename: stellantis-hackathon-unsubscribe-api-openapi.yml
  format: yaml
  label: Stellantis Hackathon Unsubscribe API
  slug: stellantis-hackathon-unsubscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-hackathon-unsubscribe-api-openapi.yml
- filename: stellantis-popup-api-openapi.yml
  format: yaml
  label: Stellantis Popup API
  slug: stellantis-popup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-popup-api-openapi.yml
- filename: stellantis-remote-api-openapi.yml
  format: yaml
  label: Stellantis Remote API
  slug: stellantis-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-remote-api-openapi.yml
- filename: stellantis-stream-api-openapi.yml
  format: yaml
  label: Stellantis Stream API
  slug: stellantis-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-stream-api-openapi.yml
consequence_counts:
  physical: 10
  read: 122
  safety-critical: 2
  write: 95
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Stellantis Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/account/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/geofencing-notifications/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fleets/{fid}/vehicles/{vid}/callbacks/{cbid}/remotes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /user/vehicles/{id}/callbacks/{cbid}/remotes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/nonRegisteredVehicles/{vehicleId}/notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/notifications/nonRegisteredUsers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/users/{userId}/nonRegisteredVehicles/{vehicleId}/notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/users/{userId}/notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/users/{userId}/vehicles/{vehicleId}/notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/vehicles/{vehicleId}/notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/vehicles/{vehicleId}/notifications/campaigns/{campaignId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/users/{userId}/notifications
operation_count: 229
overview: 'Stellantis exposes 229 API operations that an AI agent could call, of which 107 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 122 read, 95 write, 10 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Stellantis
provider_slug: stellantis
slug: stellantis-agentic-access
source_filename: stellantis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/stellantis-cloud-docg-device-management-api-openapi.yml, openapi/stellantis-cloud-notification-center-api-openapi.yml,\n  openapi/stellantis-cloud-platform-notification-webhooks-openapi.yml, openapi/stellantis-connected-car-b2b-api-openapi.yml,\n  openapi/stellantis-connected-car-b2b-webhooks-openapi.yml, openapi/stellantis-connected-car-b2c-api-openapi.yml,\n  openapi/stellantis-connected-car-b2c-webhooks-openapi.yml, openapi/stellantis-connected-vehicle-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 229\n  by_action_class:\n    acting: 107\n    connected: 122\n  by_consequence:\n    write: 95\n    read: 122\n    physical: 10\n    safety-critical: 2\n  human_in_the_loop_required:\
  \ 2\noperations:\n- path: /v1/docg/campaignCreation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/docg/campaignStart\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/docg/campaignProcessFeedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/docg/vehicleRegistrationProcessFeedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/docg/swRegistrationProcessFeedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/docg/swRegistration\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/docg/vehicleRegistration\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/docg/vehicleRegistrationUpdate\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/richContent\n  method: get\n  operationId: getV1NotificationRichcontent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification/richContent\n  method: post\n  operationId: postV1NotificationRichcontent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/template\n  method: get\n  operationId: getV1NotificationTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification/template\n  method: post\n  operationId: postV1NotificationTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/nonRegisteredVehicles/{vehicleId}/notifications\n  method: get\n  operationId: getV1NonregisteredvehiclesVehicleidNotifications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nonRegisteredVehicles/{vehicleId}/notifications\n  method: post\n  operationId: postV1NonregisteredvehiclesVehicleidNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/grouping/{group}\n  method: get\n  operationId: getV1NotificationGroupingGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification/placeholder/{key}\n  method: get\n  operationId: getV1NotificationPlaceholderKey\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification/placeholder/{key}\n  method: delete\n  operationId: deleteV1NotificationPlaceholderKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/self/config\n  method: get\n  operationId: getV1NotificationsSelfConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/self/config\n  method: patch\n  operationId: patchV1NotificationsSelfConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/notifications\n  method: get\n  operationId: getV1UsersUseridNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/notifications\n  method: post\n  operationId: postV1UsersUseridNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{vehicleId}/notifications\n  method: get\n  operationId: getV1VehiclesVehicleidNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/notifications\n  method: post\n  operationId: postV1VehiclesVehicleidNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/nonRegisteredVehicles/{vehicleId}/notifications/{platformResponseId}\n  method: get\n  operationId: getV1NonregisteredvehiclesVehicleidNotificationsPlatformresponseid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/users/{userId}/config\n  method: get\n  operationId: getV1NotificationsUsersUseridConfig\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/users/{userId}/config\n  method: patch\n  operationId: patchV1NotificationsUsersUseridConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/notifications/{platformResponseId}\n  method: get\n  operationId: getV1UsersUseridNotificationsPlatformresponseid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/notifications/{platformResponseId}\n  method: get\n  operationId: getV1VehiclesVehicleidNotificationsPlatformresponseid\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/nonRegisteredVehicles/{vehicleId}/notifications\n  method: get\n  operationId: getV1UsersUseridNonregisteredvehiclesVehicleidNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/nonRegisteredVehicles/{vehicleId}/notifications\n  method: post\n  operationId: postV1UsersUseridNonregisteredvehiclesVehicleidNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/vehicles/{vehicleId}/nickname\n  method: get\n  operationId: getV1UsersUseridVehiclesVehicleidNickname\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/vehicles/{vehicleId}/nickname\n  method: patch\n  operationId: patchV1UsersUseridVehiclesVehicleidNickname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/vehicles/{vehicleId}/notifications\n  method: get\n  operationId: getV1UsersUseridVehiclesVehicleidNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/vehicles/{vehicleId}/notifications\n  method: post\n  operationId: postV1UsersUseridVehiclesVehicleidNotifications\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/nonRegisteredVehicles/{vehicleId}/notifications/{platformResponseId}\n  method: get\n  operationId: getV1UsersUseridNonregisteredvehiclesVehicleidNotificationsPlatformresponseid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/vehicles/{vehicleId}/notifications/config\n  method: get\n  operationId: getV1UsersUseridVehiclesVehicleidNotificationsConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/vehicles/{vehicleId}/notifications/{platformResponseId}\n\
  \  method: get\n  operationId: getV1UsersUseridVehiclesVehicleidNotificationsPlatformresponseid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/vehicles/{vehicleId}/services/{serviceName}/notifications/config\n  method: get\n  operationId: getV1UsersUseridVehiclesVehicleidServicesServicenameNotificationsConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification/grouping\n  method: post\n  operationId: postV1NotificationGrouping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/placeholder\n  method:\
  \ post\n  operationId: postV1NotificationPlaceholder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/templateConfig\n  method: post\n  operationId: postV1NotificationTemplateconfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/campaigns\n  method: post\n  operationId: postV1NotificationsCampaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/nonRegisteredUsers\n  method: post\n  operationId: postV1NotificationsNonregisteredusers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notification/richContent\n  method: post\n  operationId: postV2NotificationRichcontent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notification/template\n  method: post\n  operationId: postV2NotificationTemplate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/richContent/filter\n  method: post\n  operationId: postV1NotificationRichcontentFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/template/filter\n  method: post\n  operationId: postV1NotificationTemplateFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{vehicleId}/ivmAck\n  method: post\n  operationId: postV1VehiclesVehicleidIvmack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{vehicleId}/ivmResponse\n  method: post\n  operationId: postV1VehiclesVehicleidIvmresponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/users/{userId}/notifications\n  method: post\n  operationId: postV2UsersUseridNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/default/locale/template\n  method: post\n  operationId: postV1NotificationDefaultLocaleTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/user/profile/webhooks/gigya\n  method: post\n  operationId: postV1UsersUserProfileWebhooksGigya\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/users/{userId}/vehicles/{vehicleId}/contacts\n  method: post\n  operationId: postV1UsersUseridVehiclesVehicleidContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{vehicleId}/notifications/campaigns/{campaignId}\n  method: post\n  operationId: postV1VehiclesVehicleidNotificationsCampaignsCampaignid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/users/user/profile/webhooks/gigya\n  method:\
  \ post\n  operationId: postV2UsersUserProfileWebhooksGigya\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/users/user/profile/webhooks/gigya\n  method: post\n  operationId: postV3UsersUserProfileWebhooksGigya\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/contacts/{contactId}\n  method: put\n  operationId: putV1UsersUseridContactsContactid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/contacts/{contactId}\n  method: delete\n  operationId: deleteV1UsersUseridContactsContactid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/vehicles/{vehicleId}/contacts/{contactId}/notifications/sync\n  method: put\n  operationId: putV1UsersUseridVehiclesVehicleidContactsContactidNotificationsSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/marketingNames\n\
  \  method: patch\n  operationId: patchV1NotificationMarketingnames\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/consent\n  method: patch\n  operationId: patchV1UsersUseridConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/users/{userId}/profile\n  method: patch\n  operationId: patchV1NotificationsUsersUseridProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/notifications/user/profile\n  method: patch\n  operationId: patchV1UsersUseridNotificationsUserProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/vehicles/{vehicleId}/contacts/{contactId}/notifications/config\n  method: patch\n  operationId: patchV1UsersUseridVehiclesVehicleidContactsContactidNotificationsConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/users/{userId}/vehicles/{vehicleId}/contacts/{contactId}/notifications/config\n  method: delete\n  operationId: deleteV1UsersUseridVehiclesVehicleidContactsContactidNotificationsConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/templates\n  method: delete\n  operationId: deleteV1NotificationTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/template/{notificationId}\n  method: delete\n  operationId: deleteV1NotificationTemplateNotificationid\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification/grouping/{group}/notifications/{notificationId}\n  method: delete\n  operationId: deleteV1NotificationGroupingGroupNotificationsNotificationid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notification/richContent/{notificationId}/brands/{brand}/locales/{locale}\n  method: delete\n  operationId: deleteV2NotificationRichcontentNotificationidBrandsBrandLocalesLocale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notification/template/{notificationId}/brands/{brand}/locales/{locale}\n  method: delete\n  operationId: deleteV2NotificationTemplateNotificationidBrandsBrandLocalesLocale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/webhook\n  method: post\n  operationId: postWHMsgs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/pushnotif\n\
  \  method: post\n  operationId: postPNMsgs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/websocket\n  method: post\n  operationId: postWSMsgs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{vin}\n  method: get\n  operationId: getVehiclesCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets\n  method: get\n  operationId: getFleets\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}\n  method: get\n  operationId: getFleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles\n  method: get\n  operationId: getVehiclesByDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}\n  method: get\n  operationId: getVehicleByid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/lastPosition\n  method: get\n  operationId: getCarLastPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /fleets/{fid}/vehicles/{vid}/collisions\n  method: get\n  operationId: getVehicleCollision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/collisions/{cid}\n  method: get\n  operationId: getVehicleCollisionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/maintenance\n  method: get\n  operationId: getVehicleMaintenance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/status\n  method: get\n  operationId: getFleetStatusList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/maintenances\n\
  \  method: get\n  operationId: getFleetMantenanceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/alerts\n  method: get\n  operationId: getFleetAlertList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/alerts/{aid}\n  method: get\n  operationId: getFleetAlertById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/status\n  method: get\n  operationId: getFleetVehicleStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/alerts\n  method: get\n  operationId: getVehicleAlerts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/alerts/{aid}\n  method: get\n  operationId: getFleetVehicleAlertsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/telemetry\n  method: get\n  operationId: getTelemetry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/alarms\n  method: get\n  operationId: getVehicleAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/alarms/{aid}\n  method: get\n  operationId: getVehicleAlarmsById\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/stolen\n  method: get\n  operationId: getVehicleStolenHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/stolen/{sid}\n  method: get\n  operationId: getVehicleStolenById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/vehicles/{vid}/stolen/{sid}/waypoints\n  method: get\n  operationId: getVehicleStolenIdPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/monitors\n  method: get\n  operationId: getFleetMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets/{fid}/monitors\n  method: post\n  operationId: createFleetVehicleMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fleets/{fid}/monitors/{mid}\n  method: put\n  operationId: updateFleetVehicleMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (68 KB total) ---\n# Full source: https://artifacts.apis.io/stellantis/agentic-access/stellantis-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/stellantis/agentic-access/stellantis-agentic-access.yml
summary_line: 229 operations · 107 acting · 2 human-in-the-loop
tags:
- Company
- Automotive
- Manufacturing
- Mobility
- Sustainability
---
