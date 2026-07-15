---
acting_count: 445
action_class_counts:
  acting: 445
  connected: 763
api_specs:
- filename: app-store-connect-openapi.json
  format: json
  label: App Store Connect API
  slug: app-store-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ios/main/openapi/app-store-connect-openapi.json
- filename: app-store-server-notifications-asyncapi.yml
  format: yaml
  label: App Store Server Notifications
  slug: app-store-server-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ios/main/asyncapi/app-store-server-notifications-asyncapi.yml
consequence_counts:
  physical: 100
  read: 763
  write: 345
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ios Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/appClipDefaultExperiences/{id}/relationships/releaseWithAppStoreVersion
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/appCustomProductPageLocalizations/{id}/relationships/searchKeywords
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/appEncryptionDeclarations/{id}/relationships/builds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/appPreviewSets/{id}/relationships/appPreviews
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/appScreenshotSets/{id}/relationships/appScreenshots
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/appStoreVersionLocalizations/{id}/relationships/searchKeywords
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/appStoreVersions/{id}/relationships/appClipDefaultExperience
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/appStoreVersions/{id}/relationships/build
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/apps/{id}/relationships/betaTesters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/apps/{id}/relationships/promotedPurchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/betaGroups/{id}/relationships/betaTesters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/betaGroups/{id}/relationships/betaTesters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/betaGroups/{id}/relationships/builds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/betaGroups/{id}/relationships/builds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/betaTesters/{id}/relationships/apps
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/betaTesters/{id}/relationships/betaGroups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/betaTesters/{id}/relationships/betaGroups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/betaTesters/{id}/relationships/builds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/betaTesters/{id}/relationships/builds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/builds/{id}/relationships/appEncryptionDeclaration
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/builds/{id}/relationships/betaGroups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/builds/{id}/relationships/betaGroups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/builds/{id}/relationships/individualTesters
operation_count: 1208
overview: 'iOS exposes 1208 API operations that an AI agent could call, of which 445 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 763 read, 345 write, and 100 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: iOS
provider_slug: ios
slug: ios-agentic-access
source_filename: ios-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/app-store-connect-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1208\n  by_action_class:\n    acting: 445\n    connected: 763\n  by_consequence:\n    write: 345\n    read: 763\n    physical: 100\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accessibilityDeclarations\n  method: post\n  operationId: accessibilityDeclarations_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accessibilityDeclarations/{id}\n\
  \  method: get\n  operationId: accessibilityDeclarations_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accessibilityDeclarations/{id}\n  method: patch\n  operationId: accessibilityDeclarations_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accessibilityDeclarations/{id}\n  method: delete\n  operationId: accessibilityDeclarations_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/actors\n  method: get\n  operationId: actors_getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/actors/{id}\n  method: get\n  operationId: actors_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ageRatingDeclarations/{id}\n  method: patch\n  operationId: ageRatingDeclarations_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alternativeDistributionDomains\n  method: get\n  operationId: alternativeDistributionDomains_getCollection\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionDomains\n  method: post\n  operationId: alternativeDistributionDomains_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alternativeDistributionDomains/{id}\n  method: get\n  operationId: alternativeDistributionDomains_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionDomains/{id}\n  method: delete\n  operationId: alternativeDistributionDomains_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alternativeDistributionKeys\n  method: get\n  operationId: alternativeDistributionKeys_getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionKeys\n  method: post\n  operationId: alternativeDistributionKeys_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alternativeDistributionKeys/{id}\n  method: get\n  operationId: alternativeDistributionKeys_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionKeys/{id}\n  method: delete\n  operationId: alternativeDistributionKeys_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alternativeDistributionPackageDeltas/{id}\n  method: get\n  operationId: alternativeDistributionPackageDeltas_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionPackageVariants/{id}\n  method: get\n  operationId: alternativeDistributionPackageVariants_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionPackageVersions/{id}\n  method: get\n  operationId: alternativeDistributionPackageVersions_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alternativeDistributionPackages\n  method: post\n  operationId: alternativeDistributionPackages_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alternativeDistributionPackages/{id}\n  method: get\n  operationId: alternativeDistributionPackages_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/analyticsReportInstances/{id}\n  method: get\n  operationId: analyticsReportInstances_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyticsReportRequests\n  method: post\n  operationId: analyticsReportRequests_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyticsReportRequests/{id}\n  method: get\n  operationId: analyticsReportRequests_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyticsReportRequests/{id}\n  method: delete\n  operationId: analyticsReportRequests_deleteInstance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyticsReportSegments/{id}\n  method: get\n  operationId: analyticsReportSegments_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyticsReports/{id}\n  method: get\n  operationId: analyticsReports_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/androidToIosAppMappingDetails\n  method: post\n  operationId: androidToIosAppMappingDetails_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/androidToIosAppMappingDetails/{id}\n  method: get\n  operationId: androidToIosAppMappingDetails_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/androidToIosAppMappingDetails/{id}\n  method: patch\n  operationId: androidToIosAppMappingDetails_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/androidToIosAppMappingDetails/{id}\n  method: delete\n  operationId: androidToIosAppMappingDetails_deleteInstance\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/appAvailabilities\n  method: post\n  operationId: appAvailabilitiesV2_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/appAvailabilities/{id}\n  method: get\n  operationId: appAvailabilitiesV2_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appCategories\n  method: get\n  operationId: appCategories_getCollection\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appCategories/{id}\n  method: get\n  operationId: appCategories_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appClipAdvancedExperienceImages\n  method: post\n  operationId: appClipAdvancedExperienceImages_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipAdvancedExperienceImages/{id}\n  method: get\n  operationId: appClipAdvancedExperienceImages_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/appClipAdvancedExperienceImages/{id}\n  method: patch\n  operationId: appClipAdvancedExperienceImages_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipAdvancedExperiences\n  method: post\n  operationId: appClipAdvancedExperiences_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipAdvancedExperiences/{id}\n  method: get\n  operationId: appClipAdvancedExperiences_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appClipAdvancedExperiences/{id}\n  method: patch\n  operationId: appClipAdvancedExperiences_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipAppStoreReviewDetails\n  method: post\n  operationId: appClipAppStoreReviewDetails_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipAppStoreReviewDetails/{id}\n  method: get\n  operationId: appClipAppStoreReviewDetails_getInstance\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appClipAppStoreReviewDetails/{id}\n  method: patch\n  operationId: appClipAppStoreReviewDetails_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipDefaultExperienceLocalizations\n  method: post\n  operationId: appClipDefaultExperienceLocalizations_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipDefaultExperienceLocalizations/{id}\n  method: get\n  operationId:\
  \ appClipDefaultExperienceLocalizations_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appClipDefaultExperienceLocalizations/{id}\n  method: patch\n  operationId: appClipDefaultExperienceLocalizations_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipDefaultExperienceLocalizations/{id}\n  method: delete\n  operationId: appClipDefaultExperienceLocalizations_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v1/appClipDefaultExperiences\n  method: post\n  operationId: appClipDefaultExperiences_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipDefaultExperiences/{id}\n  method: get\n  operationId: appClipDefaultExperiences_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appClipDefaultExperiences/{id}\n  method: patch\n  operationId: appClipDefaultExperiences_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipDefaultExperiences/{id}\n  method: delete\n  operationId: appClipDefaultExperiences_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipHeaderImages\n  method: post\n  operationId: appClipHeaderImages_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipHeaderImages/{id}\n  method: get\n  operationId: appClipHeaderImages_getInstance\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appClipHeaderImages/{id}\n  method: patch\n  operationId: appClipHeaderImages_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClipHeaderImages/{id}\n  method: delete\n  operationId: appClipHeaderImages_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appClips/{id}\n  method: get\n  operationId: appClips_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appCustomProductPageLocalizations\n  method: post\n  operationId: appCustomProductPageLocalizations_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appCustomProductPageLocalizations/{id}\n  method: get\n  operationId: appCustomProductPageLocalizations_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appCustomProductPageLocalizations/{id}\n  method: patch\n  operationId: appCustomProductPageLocalizations_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appCustomProductPageLocalizations/{id}\n  method: delete\n  operationId: appCustomProductPageLocalizations_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appCustomProductPageVersions\n  method: post\n  operationId: appCustomProductPageVersions_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appCustomProductPageVersions/{id}\n\
  \  method: get\n  operationId: appCustomProductPageVersions_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appCustomProductPageVersions/{id}\n  method: patch\n  operationId: appCustomProductPageVersions_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appCustomProductPages\n  method: post\n  operationId: appCustomProductPages_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/appCustomProductPages/{id}\n  method: get\n  operationId: appCustomProductPages_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appCustomProductPages/{id}\n  method: patch\n  operationId: appCustomProductPages_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appCustomProductPages/{id}\n  method: delete\n  operationId: appCustomProductPages_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/appEncryptionDeclarationDocuments\n  method: post\n  operationId: appEncryptionDeclarationDocuments_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEncryptionDeclarationDocuments/{id}\n  method: get\n  operationId: appEncryptionDeclarationDocuments_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appEncryptionDeclarationDocuments/{id}\n  method: patch\n  operationId: appEncryptionDeclarationDocuments_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEncryptionDeclarations\n  method: get\n  operationId: appEncryptionDeclarations_getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appEncryptionDeclarations\n  method: post\n  operationId: appEncryptionDeclarations_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEncryptionDeclarations/{id}\n  method: get\n  operationId: appEncryptionDeclarations_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/appEventLocalizations\n  method: post\n  operationId: appEventLocalizations_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventLocalizations/{id}\n  method: get\n  operationId: appEventLocalizations_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appEventLocalizations/{id}\n  method: patch\n  operationId: appEventLocalizations_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/appEventLocalizations/{id}\n  method: delete\n  operationId: appEventLocalizations_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventScreenshots\n  method: post\n  operationId: appEventScreenshots_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventScreenshots/{id}\n  method: get\n  operationId: appEventScreenshots_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appEventScreenshots/{id}\n  method: patch\n  operationId: appEventScreenshots_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventScreenshots/{id}\n  method: delete\n  operationId: appEventScreenshots_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventVideoClips\n  method: post\n  operationId: appEventVideoClips_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventVideoClips/{id}\n  method: get\n  operationId: appEventVideoClips_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appEventVideoClips/{id}\n  method: patch\n  operationId: appEventVideoClips_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEventVideoClips/{id}\n  method: delete\n  operationId: appEventVideoClips_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEvents\n  method: post\n  operationId: appEvents_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEvents/{id}\n  method: get\n  operationId: appEvents_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appEvents/{id}\n  method: patch\n  operationId: appEvents_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appEvents/{id}\n  method: delete\n  operationId: appEvents_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appInfoLocalizations\n  method: post\n  operationId: appInfoLocalizations_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appInfoLocalizations/{id}\n  method: get\n  operationId: appInfoLocalizations_getInstance\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appInfoLocalizations/{id}\n  method: patch\n  operationId: appInfoLocalizations_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appInfoLocalizations/{id}\n  method: delete\n  operationId: appInfoLocalizations_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appInfos/{id}\n  method: get\n  operationId: appInfos_getInstance\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appInfos/{id}\n  method: patch\n  operationId: appInfos_updateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appPreviewSets\n  method: post\n  operationId: appPreviewSets_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appPreviewSets/{id}\n  method: get\n  operationId: appPreviewSets_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appPreviewSets/{id}\n  method: delete\n  operationId: appPreviewSets_deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appPreviews\n  method: post\n  operationId: appPreviews_createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appPreviews/{id}\n  method: get\n  operationId: appPreviews_getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v\n\n# --- truncated at 32 KB (372 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/ios/refs/heads/main/agentic-access/ios-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ios/refs/heads/main/agentic-access/ios-agentic-access.yml
summary_line: 1208 operations · 445 acting
tags:
- iOS
- Apple
- Mobile
- App Store
- Push Notifications
- In-App Purchases
- Subscriptions
- Authentication
- Wallet
- Developer Platform
---
