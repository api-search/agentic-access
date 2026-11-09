---
acting_count: 37
action_class_counts:
  acting: 37
  connected: 20
api_specs:
- filename: affiliatebase-io-affiliate-coupons-api-openapi.yml
  format: yaml
  label: AffiliateBase Affiliate Coupons API
  slug: affiliatebase-io-affiliate-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-affiliate-coupons-api-openapi.yml
- filename: affiliatebase-io-affiliates-api-openapi.yml
  format: yaml
  label: AffiliateBase Affiliates API
  slug: affiliatebase-io-affiliates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-affiliates-api-openapi.yml
- filename: affiliatebase-io-api-keys-api-openapi.yml
  format: yaml
  label: AffiliateBase API Keys API
  slug: affiliatebase-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-api-keys-api-openapi.yml
- filename: affiliatebase-io-campaigns-api-openapi.yml
  format: yaml
  label: AffiliateBase Campaigns API
  slug: affiliatebase-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-campaigns-api-openapi.yml
- filename: affiliatebase-io-commissions-api-openapi.yml
  format: yaml
  label: AffiliateBase Commissions API
  slug: affiliatebase-io-commissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-commissions-api-openapi.yml
- filename: affiliatebase-io-invitations-api-openapi.yml
  format: yaml
  label: AffiliateBase Invitations API
  slug: affiliatebase-io-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-invitations-api-openapi.yml
- filename: affiliatebase-io-links-api-openapi.yml
  format: yaml
  label: AffiliateBase Links API
  slug: affiliatebase-io-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-links-api-openapi.yml
- filename: affiliatebase-io-payout-exports-api-openapi.yml
  format: yaml
  label: AffiliateBase Payout Exports API
  slug: affiliatebase-io-payout-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-payout-exports-api-openapi.yml
- filename: affiliatebase-io-payout-runs-api-openapi.yml
  format: yaml
  label: AffiliateBase Payout Runs API
  slug: affiliatebase-io-payout-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-payout-runs-api-openapi.yml
- filename: affiliatebase-io-payouts-api-openapi.yml
  format: yaml
  label: AffiliateBase Payouts API
  slug: affiliatebase-io-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-payouts-api-openapi.yml
- filename: affiliatebase-io-referrals-api-openapi.yml
  format: yaml
  label: AffiliateBase Referrals API
  slug: affiliatebase-io-referrals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/affiliatebase-io/openapi/affiliatebase-io-referrals-api-openapi.yml
consequence_counts:
  physical: 8
  read: 20
  safety-critical: 4
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Affiliatebase Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/affiliates/{affiliate_id}/promo_codes/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/api_keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/invitations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/invitations/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invitations/{id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payout_exports
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/payout_exports/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payout_exports/{payout_export_id}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payout_runs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/payout_runs/{id}/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/payout_runs/{id}/remediate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payouts/{id}/pay
operation_count: 57
overview: 'AffiliateBase exposes 57 API operations that an AI agent could call, of which 37 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 25 write, 8 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AffiliateBase
provider_slug: affiliatebase-io
slug: affiliatebase-io-agentic-access
source_filename: affiliatebase-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/affiliatebase-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 20\n    acting: 37\n  by_consequence:\n    read: 20\n    write: 25\n    safety-critical: 4\n    physical: 8\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/api_keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api_keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_keys/{id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/affiliates\n  method: get\n  operationId: listAffiliates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/affiliates\n  method: post\n  operationId: createAffiliate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{id}\n  method: get\n  operationId: getAffiliate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/affiliates/{id}\n  method: patch\n  operationId: updateAffiliate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{id}\n  method: delete\n  operationId: deleteAffiliate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/v1/affiliates/{id}/ban\n  method: post\n  operationId: banAffiliate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{id}/unban\n  method: post\n  operationId: unbanAffiliate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/coupon\n  method: get\n  operationId: getAffiliateCoupon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/affiliates/{affiliate_id}/coupon\n  method: post\n  operationId: createAffiliateCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/coupon\n  method: patch\n  operationId: regenerateAffiliateCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/coupon\n  method: delete\n  operationId: deleteAffiliateCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/coupon/sync\n  method: post\n  operationId: syncAffiliateCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{id}\n  method: patch\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{id}\n  method: delete\n  operationId: deleteCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/links\n  method: get\n  operationId: listLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/links\n  method: post\n  operationId: createLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/links/{id}\n  method: get\n  operationId: getLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/links/{id}\n  method: patch\n  operationId: updateLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/links/{id}\n  method: delete\n  operationId: deleteLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/referrals\n  method: get\n  operationId: listReferrals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/referrals\n  method: post\n  operationId: createReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/referrals/{id}\n  method: get\n  operationId: getReferral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/referrals/{id}\n  method: patch\n  operationId: updateReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/referrals/{id}\n  method: delete\n  operationId: deactivateReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/commissions\n  method: get\n  operationId: listCommissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commissions/{id}\n  method: get\n  operationId: getCommission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commissions/{id}\n  method: patch\n  operationId: updateCommission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commissions/{id}\n  method: delete\n  operationId: voidCommission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commissions/{id}/review\n  method: post\n  operationId: reviewCommissionFraud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payouts\n  method: get\n  operationId: listPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payouts/{id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payouts/{id}/pay\n\
  \  method: post\n  operationId: payPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout_exports\n  method: get\n  operationId: listPayoutExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payout_exports\n  method: post\n  operationId: createPayoutExport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /api/v1/payout_exports/{id}\n  method: get\n  operationId: getPayoutExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payout_exports/{id}\n  method: delete\n  operationId: deletePayoutExport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout_exports/{payout_export_id}/payment\n  method: post\n  operationId: markPayoutExportPaid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout_runs\n  method: post\n  operationId: createPayoutRun\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout_runs/{id}/execute\n  method: put\n  operationId: executePayoutRun\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout_runs/{id}/remediate\n  method:\
  \ put\n  operationId: remediatePayoutRun\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payout_runs/reconcile\n  method: get\n  operationId: reconcilePayoutRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invitations\n  method: get\n  operationId: listInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invitations\n  method: post\n  operationId: createInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations/{id}\n  method: get\n  operationId: getInvitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invitations/{id}\n  method: patch\n  operationId: updateInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/invitations/{id}\n  method: delete\n  operationId: deleteInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/invitations/{id}/resend\n  method: post\n  operationId: resendInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/promo_codes\n  method: get\n  operationId: listAffiliatePromoCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/affiliates/{affiliate_id}/promo_codes\n  method: post\n  operationId: assignAffiliatePromoCode\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/promo_codes/{id}\n  method: patch\n  operationId: refreshAffiliatePromoCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/affiliates/{affiliate_id}/promo_codes/{id}\n  method: delete\n  operationId: stopAffiliatePromoCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n \
  \     proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/affiliatebase-io/agentic-access/affiliatebase-io-agentic-access.yml
summary_line: 57 operations · 37 acting · 4 human-in-the-loop
tags:
- Software-as-a-Service
- Affiliate Marketing
- Stripe
- Payments
- Marketing Automation
---
