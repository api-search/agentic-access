---
acting_count: 92
action_class_counts:
  acting: 92
  connected: 61
api_specs:
- filename: aura-historia-com-administration-api-openapi.yml
  format: yaml
  label: Aura Historia Administration API
  slug: aura-historia-com-administration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-administration-api-openapi.yml
- filename: aura-historia-com-auctions-api-openapi.yml
  format: yaml
  label: Aura Historia Auctions API
  slug: aura-historia-com-auctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-auctions-api-openapi.yml
- filename: aura-historia-com-billing-api-openapi.yml
  format: yaml
  label: Aura Historia Billing API
  slug: aura-historia-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-billing-api-openapi.yml
- filename: aura-historia-com-listingsources-api-openapi.yml
  format: yaml
  label: Aura Historia Listing Sources API
  slug: aura-historia-com-listingsources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-listingsources-api-openapi.yml
- filename: aura-historia-com-newsletter-api-openapi.yml
  format: yaml
  label: Aura Historia Newsletter API
  slug: aura-historia-com-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-newsletter-api-openapi.yml
- filename: aura-historia-com-notifications-api-openapi.yml
  format: yaml
  label: Aura Historia Notifications API
  slug: aura-historia-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-notifications-api-openapi.yml
- filename: aura-historia-com-oauth-api-openapi.yml
  format: yaml
  label: Aura Historia OAuth API
  slug: aura-historia-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-oauth-api-openapi.yml
- filename: aura-historia-com-operations-api-openapi.yml
  format: yaml
  label: Aura Historia Operations API
  slug: aura-historia-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-operations-api-openapi.yml
- filename: aura-historia-com-overview-api-openapi.yml
  format: yaml
  label: Aura Historia Overview API
  slug: aura-historia-com-overview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-overview-api-openapi.yml
- filename: aura-historia-com-parties-api-openapi.yml
  format: yaml
  label: Aura Historia Parties API
  slug: aura-historia-com-parties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-parties-api-openapi.yml
- filename: aura-historia-com-partnershipapplications-api-openapi.yml
  format: yaml
  label: Aura Historia Partnership Applications API
  slug: aura-historia-com-partnershipapplications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-partnershipapplications-api-openapi.yml
- filename: aura-historia-com-partnerships-api-openapi.yml
  format: yaml
  label: Aura Historia Partnerships API
  slug: aura-historia-com-partnerships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-partnerships-api-openapi.yml
- filename: aura-historia-com-party-api-openapi.yml
  format: yaml
  label: Aura Historia Party API
  slug: aura-historia-com-party-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-party-api-openapi.yml
- filename: aura-historia-com-productlistings-api-openapi.yml
  format: yaml
  label: Aura Historia Product Listings API
  slug: aura-historia-com-productlistings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-productlistings-api-openapi.yml
- filename: aura-historia-com-search-filters-api-openapi.yml
  format: yaml
  label: Aura Historia Search Filters API
  slug: aura-historia-com-search-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-search-filters-api-openapi.yml
- filename: aura-historia-com-user-account-api-openapi.yml
  format: yaml
  label: Aura Historia User Account API
  slug: aura-historia-com-user-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-user-account-api-openapi.yml
- filename: aura-historia-com-users-api-openapi.yml
  format: yaml
  label: Aura Historia Users API
  slug: aura-historia-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-users-api-openapi.yml
- filename: aura-historia-com-watchlist-api-openapi.yml
  format: yaml
  label: Aura Historia Watchlist API
  slug: aura-historia-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aura-historia-com/openapi/aura-historia-com-watchlist-api-openapi.yml
consequence_counts:
  physical: 17
  read: 61
  safety-critical: 7
  write: 68
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Aura Historia Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/admin/parties/{party_id}/location-managers/{user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/admin/partnerships/{partnershipId}/listing-source-grants/{listingSourceId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/admin/partnerships/{partnershipId}/members/{userId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/admin/users/{userId}/access-tokens
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/admin/users/{userId}/access-tokens/{accessTokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/admin/users/{userId}/sessions/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/oauth/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/admin/partnership-applications/{partnershipApplicationId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/admin/partnership-applications/{partnershipApplicationId}/decision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/admin/partnerships/{partnershipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/admin/partnerships/{partnershipId}/listing-source-grants/{listingSourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/admin/partnerships/{partnershipId}/members/{userId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/admin/product-listings/{productListingId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/listing-sources/{listingSourceId}/product-listings/async
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/listing-sources/{listingSourceId}/product-listings/{productListingId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/listing-sources/{listing_source_id}/shipping-default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/listing-sources/{listing_source_id}/shipping-default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/listing-sources/{listing_source_id}/shipping-profiles
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/listing-sources/{listing_source_id}/shipping-profiles/{shipping_profile_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/listing-sources/{listing_source_id}/shipping-profiles/{shipping_profile_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/listing-sources/{listing_source_id}/shipping-profiles/{shipping_profile_id}/restore
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/me/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/me/partnership-applications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/me/partnership-applications/{partnershipApplicationId}
operation_count: 153
overview: 'Aura Historia exposes 153 API operations that an AI agent could call, of which 92 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read, 68 write, 17 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aura Historia
provider_slug: aura-historia-com
slug: aura-historia-com-agentic-access
source_filename: aura-historia-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/aura-historia-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 153\n  by_action_class:\n    connected: 61\n    acting: 92\n  by_consequence:\n    read: 61\n    write: 68\n    physical: 17\n    safety-critical: 7\n  human_in_the_loop_required: 7\noperations:\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOAuthAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ready\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/overview\n  method: get\n  operationId: getPublicOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auctions\n  method: get\n  operationId: listAuctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auctions/{auctionId}\n  method: get\n  operationId: getAuction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auctions/{auctionId}/product-listings\n  method: get\n  operationId: getAuctionCatalogue\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/product-listings\n  method: get\n  operationId: searchAdminProductListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/product-listings/{productListingId}\n  method: get\n  operationId: getAdminProductListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/product-listings/{productListingId}\n  method: patch\n  operationId: updateAdminProductListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/admin/product-listings/{productListingId}\n  method: delete\n  operationId: withdrawAdminProductListing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/product-listings/{productListingId}/restore\n  method: post\n  operationId: restoreAdminProductListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/auctions\n  method: get\n  operationId: adminSearchAuctions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/auctions\n  method: post\n  operationId: createAdminAuction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/auctions/{auctionId}\n  method: get\n  operationId: getAdminAuction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/auctions/{auctionId}\n  method: patch\n  operationId: updateAdminAuction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/ingestion-configurations/woocommerce\n  method: put\n  operationId: putWoocommerceListingSourceIngestionConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/ingestion-configurations/shopify\n  method: put\n  operationId: putShopifyListingSourceIngestionConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings\n\
  \  method: get\n  operationId: listPartnerProductListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listing-sources/{listingSourceId}/product-listings\n  method: post\n  operationId: postPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings\n  method: patch\n  operationId: patchPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/listing-sources/{listingSourceId}/product-listings\n  method: put\n  operationId: putPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings\n  method: delete\n  operationId: deletePartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/{productListingId}\n  method: get\n  operationId: getPartnerProductListing\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listing-sources/{listingSourceId}/product-listings/{productListingId}\n  method: patch\n  operationId: updatePartnerProductListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/{productListingId}\n  method: delete\n  operationId: withdrawPartnerProductListing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/{productListingId}/restore\n\
  \  method: post\n  operationId: restorePartnerProductListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/async\n  method: post\n  operationId: postAsyncPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/async\n  method: patch\n  operationId: patchAsyncPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/async\n  method: put\n  operationId: putAsyncPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listing-sources/{listingSourceId}/product-listings/async\n  method: delete\n  operationId: deleteAsyncPartnerProductListings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/webhooks/woocommerce/{listingSourceId}\n  method: post\n  operationId: postWoocommerceWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/loops\n  method: post\n  operationId: postLoopsPreferenceWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/product-listings/by-slug/{productListingTitleSlugId}\n  method: get\n  operationId: getProductListingByTitleSlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-listings/{productListingId}\n  method: get\n  operationId: getProductListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-listings/{productListingId}/history\n  method: get\n  operationId: getProductListingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-listings/{productListingId}/similar\n  method: get\n  operationId: getSimilarProductListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-listings\n  method: get\n  operationId: simpleSearchProductListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/search-filters\n  method: get\n  operationId: getUserSearchFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/search-filters\n  method: post\n  operationId: createUserSearchFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/search-filters/{userSearchFilterId}\n  method: get\n  operationId: getUserSearchFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/search-filters/{userSearchFilterId}\n  method: delete\n  operationId: deleteUserSearchFilter\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/search-filters/{userSearchFilterId}\n  method: patch\n  operationId: updateUserSearchFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/search-filters/{userSearchFilterId}/matches\n  method: get\n  operationId: listSearchFilterMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/search-filters/{userSearchFilterId}/matches/{productListingId}\n\
  \  method: patch\n  operationId: updateSearchFilterMatchFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/watchlist\n  method: get\n  operationId: getWatchlistProductListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/watchlist\n  method: post\n  operationId: addWatchlistProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/listing-sources\n  method: post\n  operationId: adminCreateListingSource\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/listing-sources\n  method: get\n  operationId: adminSearchListingSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/parties\n  method: post\n  operationId: adminCreateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/parties\n  method: get\n  operationId: adminSearchParties\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/parties/{partyId}\n  method: delete\n  operationId: adminDeleteParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/parties/{partyId}\n  method: patch\n  operationId: adminUpdateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/parties/{partyId}\n  method: get\n  operationId: adminGetParty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users\n  method: get\n  operationId: adminSearchUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users/{userId}\n  method: get\n  operationId: adminGetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users/{userId}\n  method: patch\n  operationId: adminPatchUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}\n  method: delete\n  operationId: adminDeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}/suspension\n  method: put\n  operationId: adminSuspendUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}/suspension\n  method: delete\n  operationId: adminUnsuspendUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}/sessions/revoke\n\
  \  method: post\n  operationId: adminRevokeUserSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/admin/users/{userId}/access-tokens\n  method: get\n  operationId: adminListUserAccessTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users/{userId}/access-tokens\n  method: delete\n  operationId: adminDeleteUserAccessTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/admin/users/{userId}/access-tokens/{accessTokenId}\n  method: delete\n  operationId: adminDeleteUserAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/account\n  method: get\n  operationId: getUserAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/me/account\n  method: patch\n  operationId: updateUserAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/access-tokens\n  method: post\n  operationId: postMyAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/access-tokens\n  method: get\n  operationId: getMyAccessTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/access-tokens\n  method: patch\n\
  \  operationId: patchMyAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/access-tokens/{accessTokenId}\n  method: get\n  operationId: getMyAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/access-tokens/{accessTokenId}\n  method: delete\n  operationId: deleteMyAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/billing/checkout\n  method: post\n  operationId: postBillingCheckout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/billing/portal\n  method: post\n  operationId: postBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/billing/manage\n  method: post\n  operationId: postBillingManage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/me/watchlist/{productListingId}\n  method: delete\n  operationId: deleteWatchlistProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/watchlist/{productListingId}\n  method: patch\n  operationId: patchWatchlistProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/me/notifications\n  method: patch\n  operationId: updateNotificationsSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/notifications\n  method: delete\n  operationId: deleteNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/notifications/all\n  method: patch\n  operationId: updateAllNotificationsSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/notifications/{notificationId}\n  method: patch\n  operationId: updateNotificationSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/notifications/{notificationId}\n  method: delete\n  operationId: deleteNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/newsletter-subscriptions\n  method: put\n  operationId: putNewsletterSubscription\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/newsletter-subscriptions/confirm\n  method: post\n  operationId: confirmNewsletterSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/listing-sources/{listingSourceId}\n  method: get\n  operationId: adminGetListingSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/listing-sources/{listingSourceId}\n  method: patch\n  operationId: adminUpdateListingSource\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/listing-sources/{listingSourceId}\n  method: delete\n  operationId: adminDeleteListingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/oauth/clients/{clientId}\n  method: get\n  operationId: getOAuthConsentClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oauth/authorize\n  method: get\n  operationId: oauthAuthorize\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oauth/token\n  method: post\n  operationId: oauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/oauth/tokens/by-third-party-code/{thirdPartyCode}\n  method: get\n  operationId: oauthTokenByThirdPartyCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oauth/revoke\n  method: post\n  operationId: oauthRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/oauth/introspect\n  method: post\n  operationId: oauthIntrospect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/oauth-clients\n  method: get\n  operationId: adminListOAuthClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/oauth-clients\n  method: post\n  operationId: adminCreateOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/admin/oauth-clients/{clientId}\n  method: get\n  operationId: adminGetOAuthClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/oauth-clients/{clientId}\n  method: patch\n  operationId: adminPatchOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/oauth-clients/{clientId}\n  method: delete\n  operationId: adminDeleteOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/listing-sources\n  method: get\n  operationId: searchPublicListingSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listing-sources/by-slug/{listingSourceSlugId}\n  method: get\n  operationId: getPublicListingSourceBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/listing-sources\n  method: get\n  operationId: getMyListingSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (49 KB total) ---\n# Full source: https://artifacts.apis.io/aura-historia-com/agentic-access/aura-historia-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/aura-historia-com/agentic-access/aura-historia-com-agentic-access.yml
summary_line: 153 operations · 92 acting · 7 human-in-the-loop
tags:
- Company
- Antiques
- Marketplace
- Search
- Software-as-a-Service
---
