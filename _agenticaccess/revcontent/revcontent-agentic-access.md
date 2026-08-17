---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 22
api_specs:
- filename: revcontent-access-api-openapi.yml
  format: yaml
  label: RevContent Access API
  slug: revcontent-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-access-api-openapi.yml
- filename: revcontent-boosts-api-openapi.yml
  format: yaml
  label: RevContent Campaigns (Boosts) API
  slug: revcontent-boosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-boosts-api-openapi.yml
- filename: revcontent-ccpa-api-openapi.yml
  format: yaml
  label: RevContent CCPA API
  slug: revcontent-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-ccpa-api-openapi.yml
- filename: revcontent-content-api-openapi.yml
  format: yaml
  label: RevContent Content API
  slug: revcontent-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-content-api-openapi.yml
- filename: revcontent-conversions-api-openapi.yml
  format: yaml
  label: RevContent Conversions API
  slug: revcontent-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-conversions-api-openapi.yml
- filename: revcontent-helpers-api-openapi.yml
  format: yaml
  label: RevContent Helpers API
  slug: revcontent-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-helpers-api-openapi.yml
- filename: revcontent-sub-accounts-api-openapi.yml
  format: yaml
  label: RevContent Sub Accounts API
  slug: revcontent-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-sub-accounts-api-openapi.yml
- filename: revcontent-targeting-api-openapi.yml
  format: yaml
  label: RevContent Targeting API
  slug: revcontent-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-targeting-api-openapi.yml
- filename: revcontent-widgets-api-openapi.yml
  format: yaml
  label: RevContent Widgets API
  slug: revcontent-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widgets-api-openapi.yml
- filename: revcontent-widget-internal-content-api-openapi.yml
  format: yaml
  label: RevContent Widget Internal Content API
  slug: revcontent-widget-internal-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-internal-content-api-openapi.yml
- filename: revcontent-widget-optimizer-api-openapi.yml
  format: yaml
  label: RevContent Widget Optimizer API
  slug: revcontent-widget-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-optimizer-api-openapi.yml
consequence_counts:
  read: 22
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Revcontent Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'RevContent exposes 43 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RevContent
provider_slug: revcontent
slug: revcontent-agentic-access
source_filename: revcontent-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/revcontent-access-api-openapi.yml, openapi/revcontent-boosts-api-openapi.yml,\n  openapi/revcontent-ccpa-api-openapi.yml, openapi/revcontent-content-api-openapi.yml, openapi/revcontent-conversions-api-openapi.yml,\n  openapi/revcontent-helpers-api-openapi.yml, openapi/revcontent-sub-accounts-api-openapi.yml,\n  openapi/revcontent-targeting-api-openapi.yml, openapi/revcontent-widget-internal-content-api-openapi.yml,\n  openapi/revcontent-widget-optimizer-api-openapi.yml, openapi/revcontent-widgets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 21\n    connected: 22\n  by_consequence:\n    write: 21\n    read: 22\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getOauthAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/account/reactivate\n  method: get\n  operationId: getReactivateAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts\n  method: get\n  operationId: getAllBoosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts\n  method: post\n  operationId: postBoostsStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/performance\n  method: get\n  operationId: getBoostPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/widgets/stats\n  method: get\n  operationId: getWidgetStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/add\n  method: post\n  operationId: postBoostAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /stats/api/v1.0/boosts/{boost_id}/archive\n  method: post\n  operationId: postBoostArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/{boost_id}/settings\n  method: post\n  operationId: postBoostSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/data_requests/submit\n  method: post\n  operationId: postSubmitCCPARequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/data_requests/data\n  method: post\n  operationId: postUserData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/data_requests/multiple_data\n  method: post\n  operationId: postUsersData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/content\n  method: get\n  operationId: getAllBoostContent\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/content\n  method: get\n  operationId: getBoostContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/content\n  method: post\n  operationId: postBoostContentUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/contents/{content_id}/widgets/stats\n  method: get\n  operationId: getContentWidgetStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/content/add\n  method: post\n  operationId: postBoostContentAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/conversions\n  method: get\n  operationId: getConversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/conversions/add\n  method: post\n  operationId: postConversionAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /stats/api/v1.0/conversions/{conversion_id}/delete\n  method: post\n  operationId: postConversionDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/conversions/{conversion_id}/update\n  method: post\n  operationId: postConversionEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/browsers\n  method: get\n  operationId: getBrowsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /stats/api/v1.0/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/dmas\n  method: get\n  operationId: getDmas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/languages\n  method: get\n  operationId: getLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/os\n  method: get\n  operationId: getOperatingSystems\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/regions\n  method: get\n  operationId: getRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/sub_accounts/add_account\n  method: post\n  operationId: addAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/sub_accounts/edit_account\n  method: post\n  operationId: editAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/sub_accounts/list_accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/sub_accounts/update_account_status\n  method: post\n  operationId: updateAccountStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/{boost_id}/widgets\n  method: get\n  operationId: getBoostWidgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/widgets\n  method: post\n\
  \  operationId: postBoostWidgets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/widgets/{widget_id}/internal_content\n  method: get\n  operationId: getWidgetInternalContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/widgets/{widget_id}/internal_content/add\n  method: post\n  operationId: postWidgetInternalContentAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/widgets/{widget_id}/internal_content/update\n\
  \  method: post\n  operationId: postWidgetInternalContentUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/{boost_id}/targets/blacklist/widgets\n  method: get\n  operationId: getTargetsOptimizerWidgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/targets/blacklist/widgets/add\n  method: post\n  operationId: postTargetsWidgetsOptimizerAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /stats/api/v1.0/boosts/{boost_id}/targets/blacklist/widgets/remove\n  method: post\n  operationId: postTargetsWidgetsOptimizerRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/widgets\n  method: get\n  operationId: getAllWidgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/widgets_geo\n  method: get\n  operationId: getAllWidgetsGeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/widgets/{widget_id}/revsub\n  method: get\n  operationId: getSubIDStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/agentic-access/revcontent-agentic-access.yml
summary_line: 43 operations · 21 acting
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
- Advertising Technology
- Campaign Management
- Audience Targeting
- Conversion Tracking
- Marketing
---
