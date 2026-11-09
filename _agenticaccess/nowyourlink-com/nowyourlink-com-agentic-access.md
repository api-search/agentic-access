---
acting_count: 76
action_class_counts:
  acting: 76
  connected: 76
api_specs:
- filename: nowyourlink-com-affiliate-api-openapi.yml
  format: yaml
  label: nowyourlink-com Affiliate API
  slug: nowyourlink-com-affiliate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-affiliate-api-openapi.yml
- filename: nowyourlink-com-agent-api-openapi.yml
  format: yaml
  label: nowyourlink-com Agent API
  slug: nowyourlink-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-agent-api-openapi.yml
- filename: nowyourlink-com-ask-api-openapi.yml
  format: yaml
  label: nowyourlink-com Ask API
  slug: nowyourlink-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-ask-api-openapi.yml
- filename: nowyourlink-com-checkout-sessions-api-openapi.yml
  format: yaml
  label: nowyourlink-com Checkout Sessions API
  slug: nowyourlink-com-checkout-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-checkout-sessions-api-openapi.yml
- filename: nowyourlink-com-sandbox-api-openapi.yml
  format: yaml
  label: nowyourlink-com Sandbox API
  slug: nowyourlink-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-sandbox-api-openapi.yml
- filename: nowyourlink-com-spotlight-api-openapi.yml
  format: yaml
  label: nowyourlink-com Spotlight API
  slug: nowyourlink-com-spotlight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-spotlight-api-openapi.yml
- filename: nowyourlink-com-spotlights-api-openapi.yml
  format: yaml
  label: nowyourlink-com Spotlights API
  slug: nowyourlink-com-spotlights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowyourlink-com/openapi/nowyourlink-com-spotlights-api-openapi.yml
consequence_counts:
  physical: 22
  read: 76
  safety-critical: 4
  write: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Nowyourlink Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/agent/account/notification-preferences
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/agent/account/notification-preferences
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/agent/connections/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/agent/connections/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/affiliate/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/affiliate/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions/{checkout_session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions/{checkout_session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions/{checkout_session_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions/{checkout_session_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions/{checkout_session_id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_sessions/{checkout_session_id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/account/data-erasure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/account/data-erasure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/agent/account/marketing-consent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/agent/account/marketing-consent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/affiliate/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/affiliate/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/agent/billing/payment-methods/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/agent/billing/payment-methods/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/billing/payment-methods/{id}/default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/billing/payment-methods/{id}/default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/agent/videos/{asset_id}
operation_count: 152
overview: 'nowyourlink-com exposes 152 API operations that an AI agent could call, of which 76 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 76 read, 50 write, 22 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: nowyourlink-com
provider_slug: nowyourlink-com
slug: nowyourlink-com-agentic-access
source_filename: nowyourlink-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/nowyourlink-com-openapi.json, openapi/nowyourlink-com-preview-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 152\n  by_action_class:\n    connected: 76\n    acting: 76\n  by_consequence:\n    read: 76\n    physical: 22\n    write: 50\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/sandbox\n  method: get\n  operationId: getSandboxExample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlight\n  method: get\n  operationId: getCurrentSpotlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlights\n  method: get\n  operationId: listSpotlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout_sessions\n  method: post\n  operationId: createMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}\n  method: get\n  operationId: getMetricsCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /checkout_sessions/{checkout_session_id}\n  method: post\n  operationId: updateMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}/complete\n  method: post\n  operationId: completeMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}/cancel\n\
  \  method: post\n  operationId: cancelMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}/resource\n  method: get\n  operationId: getPurchasedMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: get\n  operationId: askPublicSpotlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: askPublicSpotlightsPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/spotlights/batch\n  method: get\n  operationId: batchGetSpotlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlights/{day}/metrics\n  method: get\n  operationId: getSpotlightMetricsPaid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlights/{day}\n  method: get\n  operationId: getSpotlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/jobs\n  method: post\n\
  \  operationId: createSandboxJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/jobs/{jobId}\n  method: get\n  operationId: getSandboxJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/me\n  method: get\n  operationId: getAgentAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/bids\n  method: get\n  operationId: listAgentBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - bids:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/agent/bids\n  method: post\n  operationId: createAgentBid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bids:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/bids/{bidId}/increase\n  method: post\n  operationId: increaseAgentBid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bids:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives\n  method: get\n  operationId: listAgentCreatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creatives:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/creatives\n  method: post\n  operationId: createAgentCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/upload\n  method: post\n  operationId: uploadAgentCreativeAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/{id}\n  method: get\n  operationId: getAgentCreative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - creatives:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/creatives/{id}\n  method: patch\n  operationId: updateAgentCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/{id}\n  method: delete\n  operationId: delete_creative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/{id}/submit\n  method: post\n  operationId: submitAgentCreative\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/invoices\n  method: get\n  operationId: listAgentInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - invoices:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/affiliate/stats\n  method: get\n  operationId: getAffiliateStatsSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/affiliate/links\n  method: get\n  operationId: getAffiliateLinksSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/affiliate/me\n  method: get\n  operationId: getAffiliatePartnerSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/affiliate/me\n  method: post\n  operationId: activateAffiliatePartnerSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/affiliate/me\n  method: patch\n  operationId: configureAffiliatePostbackSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/affiliate/payouts\n\
  \  method: get\n  operationId: listAffiliatePayoutsSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/affiliate/payouts\n  method: post\n  operationId: requestAffiliatePayoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/affiliate/connect\n  method: get\n  operationId: getAffiliateConnectSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/affiliate/connect\n  method: post\n  operationId: startAffiliateConnectSession\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/affiliate/stats\n  method: get\n  operationId: getAffiliateStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - affiliate:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/affiliate/links\n  method: get\n  operationId: getAffiliateLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - affiliate:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/affiliate/me\n  method: get\n  operationId: getAffiliatePartner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - affiliate:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/agent/affiliate/me\n  method: post\n  operationId: activateAffiliatePartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - affiliate:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/affiliate/me\n  method: patch\n  operationId: configureAffiliatePostback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - affiliate:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/affiliate/payouts\n  method: get\n  operationId: listAffiliatePayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - affiliate:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/affiliate/payouts\n  method: post\n  operationId: requestAffiliatePayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - affiliate:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/affiliate/connect\n  method: get\n  operationId: getAffiliateConnect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - affiliate:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/affiliate/connect\n  method: post\n  operationId: startAffiliateConnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - affiliate:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/affiliate/register\n  method: post\n  operationId: registerAffiliatePartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/auctions\n  method: get\n  operationId: list_auctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - bids:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/auctions/{day}\n  method: get\n  operationId: get_auction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - bids:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/bids/history\n  method: get\n  operationId: list_bid_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - bids:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/creatives/{id}/download\n  method: get\n  operationId: get_creative_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creatives:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/billing/payment-methods\n  method: get\n  operationId: list_payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/billing/payment-methods/{id}/default\n  method: post\n  operationId: set_default_payment_method\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/billing/payment-methods/{id}\n  method: delete\n  operationId: remove_payment_method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/billing/portal\n  method: post\n  operationId: open_billing_portal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/account/passkeys\n  method: get\n  operationId: list_passkeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - security:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/account/passkeys/{id}\n  method: delete\n  operationId: remove_passkey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - security:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/account/marketing-consent\n  method: post\n  operationId: request_marketing_consent\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/account/marketing-consent\n  method: delete\n  operationId: withdraw_marketing_consent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/account/data-export\n  method: post\n  operationId: request_data_export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - privacy:write\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/account/data-erasure\n  method: post\n  operationId: request_account_erasure\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - privacy:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/connections\n  method: get\n  operationId: list_agent_connections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/connections/{id}\n  method: delete\n  operationId: revoke_agent_connection\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/account/actions\n  method: get\n  operationId: prepare_account_action\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/account/settings\n  method: get\n  operationId: get_account_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/account/company-profile\n  method: patch\n  operationId: update_company_profile\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/account/notification-preferences\n  method: patch\n  operationId: set_notification_preference\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/reports\n  method: get\n  operationId: list_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/reports/{day}\n\
  \  method: get\n  operationId: get_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/spotlights/{day}/stats\n  method: get\n  operationId: get_spotlight_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/videos\n  method: post\n  operationId: start_video_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/videos/{asset_id}/parts\n  method: post\n  operationId: get_video_upload_urls\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/videos/{asset_id}/complete\n  method: post\n  operationId: complete_video_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/videos/{asset_id}/status\n  method: get\n  operationId: get_video_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creatives:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/videos/{asset_id}\n\
  \  method: delete\n  operationId: abort_video_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/{id}/video\n  method: post\n  operationId: replace_creative_video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox\n  method: get\n  operationId: getSandboxExample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlight\n  method: get\n  operationId: getCurrentSpotlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlights\n  method: get\n  operationId: listSpotlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout_sessions\n  method: post\n  operationId: createMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}\n  method:\
  \ get\n  operationId: getMetricsCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout_sessions/{checkout_session_id}\n  method: post\n  operationId: updateMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}/complete\n  method: post\n  operationId: completeMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}/cancel\n  method: post\n  operationId: cancelMetricsCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{checkout_session_id}/resource\n  method: get\n  operationId: getPurchasedMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: get\n  operationId: askPublicSpotlights\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: askPublicSpotlightsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/spotlights/batch\n  method: get\n  operationId: batchGetSpotlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlights/{day}/metrics\n  method: get\n  operationId: getSpotlightMetricsPaid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spotlights/{day}\n  method: get\n  operationId:\
  \ getSpotlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/jobs\n  method: post\n  operationId: createSandboxJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/jobs/{jobId}\n  method: get\n  operationId: getSandboxJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/me\n  method: get\n  operationId: getAgentAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/agent/bids\n  method: get\n  operationId: listAgentBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - bids:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/bids\n  method: post\n  operationId: createAgentBid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bids:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/bids/{bidId}/increase\n  method: post\n  operationId: increaseAgentBid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bids:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/agent/creatives\n  method: get\n  operationId: listAgentCreatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creatives:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/creatives\n  method: post\n  operationId: createAgentCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/upload\n  method: post\n  operationId: uploadAgentCreativeAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/{id}\n  method: get\n  operationId: getAgentCreative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - creatives:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/creatives/{id}\n  method: patch\n  operationId: updateAgentCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/creatives/{id}\n  method: delete\n  operationId: delete_creative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - creatives:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (47 KB total) ---\n# Full source: https://artifacts.apis.io/nowyourlink-com/agentic-access/nowyourlink-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/nowyourlink-com/agentic-access/nowyourlink-com-agentic-access.yml
summary_line: 152 operations · 76 acting · 4 human-in-the-loop
tags:
- Advertising
- Marketplace
- Auctions
- Technology
---
