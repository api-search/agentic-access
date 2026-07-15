---
acting_count: 323
action_class_counts:
  acting: 323
  connected: 268
api_specs:
- filename: flipdish-apps-openapi.json
  format: json
  label: Flipdish Apps & Channels API
  slug: apps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-apps-openapi.json
- filename: flipdish-catalog-openapi.json
  format: json
  label: Flipdish Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-catalog-openapi.json
- filename: flipdish-customers-openapi.json
  format: json
  label: Flipdish Customers & Accounts API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-customers-openapi.json
- filename: flipdish-devices-openapi.json
  format: json
  label: Flipdish Devices API
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-devices-openapi.json
- filename: flipdish-marketing-openapi.json
  format: json
  label: Flipdish Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-marketing-openapi.json
- filename: flipdish-menus-openapi.json
  format: json
  label: Flipdish Menus API
  slug: menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-menus-openapi.json
- filename: flipdish-orders-openapi.json
  format: json
  label: Flipdish Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-orders-openapi.json
- filename: flipdish-payments-openapi.json
  format: json
  label: Flipdish Payments & Payouts API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-payments-openapi.json
- filename: flipdish-platform-openapi.json
  format: json
  label: Flipdish Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-platform-openapi.json
- filename: flipdish-stores-openapi.json
  format: json
  label: Flipdish Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-stores-openapi.json
consequence_counts:
  physical: 27
  read: 268
  safety-critical: 10
  write: 286
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Flipdish Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/accounts/password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/accounts/password/resetpin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/accounts/passwordreset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/lightspeed/{storeId}/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/orders/{id}/dispatch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/stores/{storeId}/businesshoursoverrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1.0/stores/{storeId}/businesshoursoverrides/{businessHoursOverrideId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/users/{userId}/ResetMfa
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1.0/{appId}/authorizationtokens/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.0/{appId}/features/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/apps/{appId}/SendPushNotification/{customerId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/auditlogs/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/menus/{menuId}/sectiondisplayorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/menus/{menuId}/sections/{menuSectionId}/sectionitemdisplayorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/menus/{menuId}/sections/{menuSectionId}/sectionitems/{menuSectionItemId}/setorder/{destinationDisplayOrder}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/orders/{id}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/orders/{id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/orders/{id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/orders/{orderId}/deliveryinfo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/orders/{orderId}/fulfillment/state
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/orders/{orderId}/tracking/{deliveryTrackingStatus}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/stores/{storeId}/order-batching-configuration
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/stores/{storeId}/preorderconfig/{deliveryType}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/stores/{storeId}/preorderconfig/{deliveryType}/enabled
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/stores/{storeId}/servicecharge
operation_count: 591
overview: 'Flipdish exposes 591 API operations that an AI agent could call, of which 323 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 268 read, 286 write, 27 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flipdish
provider_slug: flipdish
slug: flipdish-agentic-access
source_filename: flipdish-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/flipdish-apps-openapi.json, openapi/flipdish-catalog-openapi.json, openapi/flipdish-customers-openapi.json,\n  openapi/flipdish-devices-openapi.json, openapi/flipdish-marketing-openapi.json, openapi/flipdish-menus-openapi.json,\n  openapi/flipdish-orders-openapi.json, openapi/flipdish-payments-openapi.json, openapi/flipdish-platform-openapi.json,\n  openapi/flipdish-stores-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 591\n  by_action_class:\n    connected: 268\n    acting: 323\n  by_consequence:\n    read: 268\n    write: 286\n    physical: 27\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /api/v1.0/apps/{appId}\n  method: get\n  operationId:\
  \ GetApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/{appId}/name\n  method: get\n  operationId: GetAppName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/supportedcountries\n  method: get\n  operationId: GetSupportedCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/{appId}/compliance\n  method: get\n  operationId: GetCompliance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/{appId}/compliance\n  method:\
  \ post\n  operationId: SetCompliance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/panacea/url\n  method: get\n  operationId: GetPanaceaVanityUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/{appId}/panacea/url\n  method: post\n  operationId: SetPanaceaVanityUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/v1.0/apps/{whitelabelId}/lookup\n  method: get\n  operationId: LookupByWhitelabelId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/{appId}/hostnamestatus\n  method: get\n  operationId: GetAppHostnameStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps\n  method: get\n  operationId: GetApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps\n  method: post\n  operationId: CreateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/panacea/url/available\n  method: get\n  operationId: IsPanaceaVanityUrlAvailable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/apps/{appId}/logo\n  method: post\n  operationId: UploadAppLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/config\n  method: post\n  operationId: SetAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/appstorename\n  method: post\n  operationId: SetAppStoreName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/orgId/{orgId}\n  method: post\n  operationId: Apps_SetPropertyId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/config/languages\n\
  \  method: post\n  operationId: SetAppLanguages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/SendPushNotification/{customerId}\n  method: post\n  operationId: SendPushNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/third-party-integrations\n  method: post\n  operationId: SetThirdPartyIntegrations\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/hostname\n  method: post\n  operationId: SetAppHostname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/apps/{appId}/nextgenweb\n  method: post\n  operationId: ToggleNextGenWeb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/v1.0/appstore/apps/{appStoreAppId}\n  method: get\n  operationId: GetAppStoreApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/appstore/apps\n  method: get\n  operationId: GetAppStoreApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/appstore/apps\n  method: get\n  operationId: GetConfiguredApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}\n  method: get\n  operationId: GetConfiguredAppSingleApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/appstore/oauthresponse/{appStoreAppId}/responsecode\n  method: get\n  operationId: AppStoreConfigurations_AppStoreHandleOauthResponseCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/config/{configId}\n  method: get\n  operationId: GetAppStoreConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/config/{configId}\n  method: put\n  operationId: UpdateAppStoreConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/config/{configId}\n  method: delete\n  operationId: DeleteAppStoreConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/config\n  method: post\n  operationId: CreateAppStoreConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/config/{configId}/action\n\
  \  method: post\n  operationId: ExecuteConfigurationAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/config/{configId}/updatesettings\n  method: post\n  operationId: UpdateAppStoreConfigSettingValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}/external_product\n  method: get\n  operationId: GetAppExternalProduct\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}/external_product\n  method: put\n  operationId: UpdateExternalProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}/external_function_signing_key\n  method: get\n  operationId: GetExternalFunctionSigningKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}\n  method: put\n\
  \  operationId: UpdateAppStoreApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}\n  method: delete\n  operationId: DeleteAppStoreApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}/verification\n  method: put\n  operationId: AppVerificationUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps\n  method: post\n  operationId: CreateAppStoreApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/oauthclients/{oauthAppId}/appstore/apps/{appStoreAppId}/logo\n  method: post\n  operationId: UploadAppStoreAppLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/appstore/apps/{appStoreAppId}/entitlements\n  method: get\n  operationId: GetAppStoreAppEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels\n  method: get\n  operationId: GetChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels/{id}\n  method: get\n  operationId: GetChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels/assigned-channels\n  method: get\n  operationId: GetAssignedChannels\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels/available-channels\n  method: get\n  operationId: GetAvailableChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels/{channelId}/stores\n  method: get\n  operationId: GetStoresBySalesChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels/{channelId}/stores\n  method: delete\n  operationId: DetachAllStoresFromSalesChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/channels/{channelId}/assigned-stores\n  method: get\n  operationId: GetStoresAssignedToChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/channels/{channelId}/assign-appId\n  method: post\n  operationId: AssignAppIdToSalesChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/channels/{channelId}/stores/{storeId}\n  method: post\n  operationId: AttachStoreToSalesChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/channels/{channelId}/stores/{storeId}\n  method: delete\n  operationId: DetachStoreFromSalesChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/channels/assign-store\n  method: post\n  operationId: AssignStoreToChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/v1.0/{appId}/channels/unassign-store\n  method: delete\n  operationId: UnassignStoreFromChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/FirebaseApp/{whitelabelId}\n  method: get\n  operationId: FirebaseApps_GetFirebaseApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/FirebaseApp\n  method: post\n  operationId: FirebaseApps_AddFirebaseApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/FirebaseApp/{whiteLabelId}\n  method: delete\n  operationId: FirebaseApps_DeleteFirebaseApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/submission/details\n  method: get\n  operationId: GetSubmissionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/mobileapps/{appId}/saleschannel/details\n  method: get\n  operationId: GetAppConfigSalesChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/mobileapps/{appId}/submission/{submissionId}/status\n  method: get\n  operationId: GetSubmissionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/mobileapps/{appId}/submission/{submissionId}/status\n  method: post\n  operationId: UpdateSubmissionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/statistics\n  method: get\n  operationId: GetStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/mobileapps/{appId}/submission\n  method: post\n  operationId: Submission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/resubmission\n  method: post\n  operationId: Resubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/saleschannel\n  method: post\n  operationId: UpdateAppConfigSalesChannel\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/submission/image\n  method: post\n  operationId: UploadImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/submission/{submissionId}/publish\n  method: post\n  operationId: Publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/mobileapps/{appId}/submission/{submissionId}/unpublish\n  method: post\n  operationId: Unpublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/website/index\n  method: get\n  operationId: GetIndexConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/website/index\n  method: post\n  operationId: SetIndexConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/website/dnscheck\n  method: get\n  operationId: Website_CheckNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/website/testimonial\n  method: post\n  operationId: AddTestimonial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/website/image/{imageLocation}\n  method: post\n  operationId: UploadWebsiteImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/website/testimonial/{testimonialId}\n  method: post\n  operationId: EditTestimonial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/website/testimonial/{testimonialId}\n  method: delete\n  operationId: DeleteTestimonial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/v1.0/{appId}/website/image/{imageId}\n  method: delete\n  operationId: DeleteWebsiteImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelbuilds/health\n  method: get\n  operationId: HealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/whitelabelbuilds/{appId}/android\n  method: post\n  operationId: SubmitAndroidBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelbuilds/ios/multiple\n  method: post\n  operationId: SubmitIosApps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelbuilds/{appId}/ios\n  method: post\n  operationId: SubmitIosBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelbuilds/android/multiple\n  method: post\n  operationId: SubmitAndroidApps\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelconfig/health\n  method: get\n  operationId: HealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/whitelabelconfig/id/{wlid}\n  method: get\n  operationId: GetWhiteLabelConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/whitelabelconfig/name/{appId}\n  method: get\n  operationId: GetWhiteLabelConfigByAppNameId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/whitelabelconfig/{appId}/general\n  method: get\n  operationId: GetAppGeneralConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/whitelabelconfig/{appId}/general\n  method: post\n  operationId: UpdateAppGeneralConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelconfig/{appId}/appstore\n  method: get\n  operationId: GetAppStoreConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1.0/whitelabelconfig/{appId}/appstore\n  method: post\n  operationId: UpdateAppStoreConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelconfig/{appId}/playstore\n  method: get\n  operationId: GetPlayStoreConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/whitelabelconfig/{appId}/playstore\n  method: post\n  operationId: UpdatePlayStoreConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/whitelabelconfig/{appId}/app-store-icon\n  method: post\n  operationId: UploadAppStoreIcon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/menus/catalog-changes/summaries\n  method: get\n  operationId: GetPendingMenuChangesSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/menus/catalog-changes\n  method: get\n  operationId: GetPendingMenuChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/menus/catalog-changes/publish\n  method: post\n  operationId: PublishPendingMenuChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/{appId}/catalog/groups/{catalogItemId}\n  method: get\n  operationId: GetGroupById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/{appId}/catalog/groups/{catalogItemId}\n  method: post\n  operationId: UpdateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    a\n\n# --- truncated at 32 KB (197 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/agentic-access/flipdish-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/agentic-access/flipdish-agentic-access.yml
summary_line: 591 operations · 323 acting · 10 human-in-the-loop
tags:
- Restaurant
- Online Ordering
- Mobile Apps
- Point of Sale
- Orders
- Menu
- Payments
- Webhooks
---
