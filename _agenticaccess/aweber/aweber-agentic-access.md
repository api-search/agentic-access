---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 38
api_specs:
- filename: aweber-accounts-api-openapi.yml
  format: yaml
  label: AWeber Accounts API
  slug: aweber-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-accounts-api-openapi.yml
- filename: aweber-broadcasts-api-openapi.yml
  format: yaml
  label: AWeber Broadcasts API
  slug: aweber-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-broadcasts-api-openapi.yml
- filename: aweber-campaigns-api-openapi.yml
  format: yaml
  label: AWeber Campaigns API
  slug: aweber-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-campaigns-api-openapi.yml
- filename: aweber-custom-fields-api-openapi.yml
  format: yaml
  label: AWeber Custom Fields API
  slug: aweber-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-custom-fields-api-openapi.yml
- filename: aweber-landing-pages-api-openapi.yml
  format: yaml
  label: AWeber Landing Pages API
  slug: aweber-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-landing-pages-api-openapi.yml
- filename: aweber-lists-api-openapi.yml
  format: yaml
  label: AWeber Lists API
  slug: aweber-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-lists-api-openapi.yml
- filename: aweber-segments-api-openapi.yml
  format: yaml
  label: AWeber Segments API
  slug: aweber-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-segments-api-openapi.yml
- filename: aweber-subscribers-api-openapi.yml
  format: yaml
  label: AWeber Subscribers API
  slug: aweber-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-subscribers-api-openapi.yml
- filename: aweber-integrations-api-openapi.yml
  format: yaml
  label: AWeber Integrations API
  slug: aweber-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-integrations-api-openapi.yml
- filename: aweber-beta-endpoints-api-openapi.yml
  format: yaml
  label: AWeber Beta Endpoints API
  slug: aweber-beta-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-beta-endpoints-api-openapi.yml
- filename: aweber-oauth-1-0a-reference-api-openapi.yml
  format: yaml
  label: AWeber OAuth 1.0a Reference API
  slug: aweber-oauth-1-0a-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-oauth-1-0a-reference-api-openapi.yml
- filename: aweber-oauth-2-0-reference-api-openapi.yml
  format: yaml
  label: AWeber OAuth 2.0 Reference API
  slug: aweber-oauth-2-0-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-oauth-2-0-reference-api-openapi.yml
- filename: aweber-webforms-api-openapi.yml
  format: yaml
  label: AWeber Webforms API
  slug: aweber-webforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-webforms-api-openapi.yml
consequence_counts:
  physical: 1
  read: 38
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Aweber Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/lists/{listId}/purchases
operation_count: 57
overview: 'AWeber exposes 57 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 17 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWeber
provider_slug: aweber
slug: aweber-agentic-access
source_filename: aweber-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/aweber-accounts-api-openapi.yml, openapi/aweber-authentication-api-openapi.yml,\n  openapi/aweber-beta-api-openapi.yml, openapi/aweber-broadcasts-api-openapi.yml, openapi/aweber-campaigns-api-openapi.yml,\n  openapi/aweber-custom-fields-api-openapi.yml, openapi/aweber-integrations-api-openapi.yml,\n  openapi/aweber-landing-pages-api-openapi.yml, openapi/aweber-lists-api-openapi.yml, openapi/aweber-segments-api-openapi.yml,\n  openapi/aweber-subscribers-api-openapi.yml, openapi/aweber-web-forms-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 38\n    acting: 19\n  by_consequence:\n    read: 38\n    write: 17\n    safety-critical:\
  \ 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/request_token\n  method: post\n  operationId: getARequestToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/access_token\n  method: post\n  operationId: getAnAccessToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token\n  method: post\n  operationId: getAToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/revoke\n  method: post\n  operationId: revokeAToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /analytics/reports/broadcasts-links\n\
  \  method: get\n  operationId: getBroadcastLinksAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/broadcasts\n  method: get\n  operationId: getBroadcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/broadcasts\n  method: post\n  operationId: createBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}\n  method:\
  \ get\n  operationId: getBroadcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}\n  method: put\n  operationId: updateBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}\n  method: delete\n  operationId: deleteBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}/cancel\n  method: post\n  operationId: cancelScheduledBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/total\n  method: get\n  operationId: getTotalBroadcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}/schedule\n  method: post\n  operationId: scheduleBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - email.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}/opens\n  method: get\n  operationId: getBroadcastOpens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/broadcasts/{broadcastId}/clicks\n  method: get\n  operationId: getBroadcastClicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/campaigns\n  method: get\n  operationId: getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/campaigns/{campaignType}{campaignId}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/campaigns?ws.op=find\n  method: get\n  operationId: findCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/campaigns/b{campaignId}/stats\n  method: get\n  operationId: getBroadcastStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /accounts/{accountId}/lists/{listId}/campaigns/b{campaignId}/stats/{statsId}\n  method: get\n  operationId: getBroadcastStatistic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/custom_fields\n  method: get\n  operationId: getCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/custom_fields\n  method: post\n  operationId: addCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - list.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /accounts/{accountId}/lists/{listId}/custom_fields/{customFieldId}\n  method: get\n  operationId: getCustomField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/custom_fields/{customFieldId}\n  method: delete\n  operationId: deleteCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - list.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/custom_fields/{customFieldId}\n  method: patch\n  operationId: updateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - list.write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/integrations\n  method: get\n  operationId: getIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/integrations/{integrationId}\n  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/landing_pages\n  method: get\n  operationId: getLandingPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - landing-page.read\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /accounts/{accountId}/lists/{listId}/landing_pages/{landingPageId}\n  method: get\n  operationId: getLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists\n  method: get\n  operationId: getLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}\n  method: get\n  operationId: getList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists?ws.op=find\n  method: get\n  operationId: findLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/tags\n  method: get\n  operationId: getTagsForList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/segments\n  method: get\n  operationId: getSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/segments/{segmentId}\n  method: get\n  operationId: getSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/subscribers\n  method: get\n  operationId:\
  \ getSubscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - subscriber.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/subscribers\n  method: post\n  operationId: addSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - subscriber.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/subscribers\n  method: delete\n  operationId: deleteSubscriberByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - subscriber.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/subscribers\n  method: patch\n  operationId: updateSubscriberByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - subscriber.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/subscribers/{subscriberId}\n  method: get\n  operationId: getSubscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - subscriber.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/subscribers/{subscriberId}\n  method: post\n  operationId: moveSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ subscriber.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/subscribers/{subscriberId}\n  method: delete\n  operationId: deleteSubscriberByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - subscriber.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/subscribers/{subscriberId}\n  method: patch\n  operationId: updateSubscriberByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - subscriber.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/lists/{listId}/subscribers?ws.op=find\n  method: get\n  operationId: findSubscribersForList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - subscriber.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}?ws.op=findSubscribers\n  method: get\n  operationId: findSubscribersForAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - subscriber.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/subscribers/{subscriberId}?ws.op=getActivity\n  method: get\n  operationId: getSubscriberActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - subscriber.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /accounts/{accountId}/lists/{listId}/purchases\n  method: post\n  operationId: createAPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - subscriber.read\n    - subscriber.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}?ws.op=getWebForms\n  method: get\n  operationId: getWebformsForAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}?ws.op=getWebFormSplitTests\n  method: get\n  operationId: getSplitTestsForAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/web_forms\n  method: get\n  operationId: getWebformsForList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/web_forms/{webformId}\n  method: get\n  operationId: getWebformForList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/web_form_split_tests\n  method: get\n  operationId: getSplitTestsForList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/web_form_split_tests/{splitTestId}\n  method: get\n  operationId:\
  \ getSplitTestForList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/web_form_split_tests/{splitTestId}/components\n  method: get\n  operationId: getSplitTestComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/lists/{listId}/web_form_split_tests/{splitTestId}/components/{splitTestComponentId}\n  method: get\n  operationId: getSplitTestComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - list.read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/agentic-access/aweber-agentic-access.yml
summary_line: 57 operations · 19 acting · 1 human-in-the-loop
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
- Web Forms
- Segments
- Webhook
- Authentication
- Small Business
---
