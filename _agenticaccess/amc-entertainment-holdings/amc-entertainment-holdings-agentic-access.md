---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 56
api_specs:
- filename: amc-theatres-api-openapi.yml
  format: yaml
  label: AMC Theatres API
  slug: amc-theatres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-theatres-api-openapi.yml
consequence_counts:
  physical: 16
  read: 56
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amc Entertainment Holdings Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/fee-waiver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v3/orders/{order-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orders/{order-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{order-id}/failed-payment-auths
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{order-id}/loyalty-rewards-application
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orders/{order-id}/loyalty-rewards-application
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{order-id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orders/{order-id}/payments/{line-number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{order-id}/products
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v3/orders/{order-id}/products/{line-number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/orders/{order-id}/products/{line-number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orders/{order-id}/products/{line-number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{order-id}/products/{line-number}/sms-ticket-confirmation/{phone-number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{order-id}/refresh-expiration
operation_count: 79
overview: 'AMC Entertainment Holdings exposes 79 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 56 read, 7 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AMC Entertainment Holdings
provider_slug: amc-entertainment-holdings
slug: amc-entertainment-holdings-agentic-access
source_filename: amc-entertainment-holdings-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amc-theatres-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 79\n  by_action_class:\n    connected: 56\n    acting: 23\n  by_consequence:\n    read: 56\n    physical: 16\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/theatres\n  method: get\n  operationId: listTheatres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/{idOrSlug}\n  method: get\n  operationId: getTheatre\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/views/now-playing/wwm-release-number/{wwm-release-number}\n\
  \  method: get\n  operationId: listTheatresByWwmRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/{theatre-number}/showtimes\n  method: get\n  operationId: listTheatreShowtimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/{theatre-number}/showtimes/{date}\n  method: get\n  operationId: listTheatreShowtimesByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/{theatre-number}/showtimes/{date}/views/embargoed\n  method: get\n  operationId: listEmbargoedShowtimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/{theatre-number}/movies/{movie-id}/earliest-showtime\n\
  \  method: get\n  operationId: getEarliestShowtime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/theatres/{theatre-number}/seating-layouts\n  method: get\n  operationId: listTheatreSeatingLayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/showtimes/{id}\n  method: get\n  operationId: getShowtime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/showtimes/views/current-location/{date}/{latitude}/{longitude}\n  method: get\n  operationId: listShowtimesByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies\n  method: get\n  operationId:\
  \ listMovies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/views/now-playing\n  method: get\n  operationId: listMoviesNowPlaying\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/views/advance\n  method: get\n  operationId: listMoviesAdvance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/views/coming-soon\n  method: get\n  operationId: listMoviesComingSoon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/views/active\n  method: get\n  operationId: listMoviesActive\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/views/all/active\n  method: get\n  operationId: listMoviesAllActive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/views/on-demand\n  method: get\n  operationId: listMoviesOnDemand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/{idOrSlug}\n  method: get\n  operationId: getMovie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/{id}/on-demand/similar\n  method: get\n  operationId: listSimilarOnDemandMovies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/movies/internal-release/{id}\n  method: get\n  operationId: getMovieByInternalRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/states/{state-name}\n  method: get\n  operationId: listLocationsByState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/theatres/{theatre-name}\n  method: get\n  operationId: listLocationsByTheatreName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/location-suggestions\n  method: get\n  operationId: listLocationSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets\n\
  \  method: get\n  operationId: listMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/states\n  method: get\n  operationId: listStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/states/{state-slug}\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/seating-layouts/{theatre-number}/{performance-number}\n  method: get\n  operationId: getSeatingLayoutForPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/media/{media-type}/{media-id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/media/{resource-type}/{resource-id}/{media-type}\n  method: get\n  operationId: listMediaForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/media/images/content-types\n  method: get\n  operationId: listImageContentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/media/videos/content-types\n  method: get\n  operationId: listVideoContentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/images/sizes\n  method: get\n  operationId: listImageSizes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/record\n  method: post\n  operationId: recordOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders/{order-id}\n  method: put\n  operationId: updateOrderContact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/token-{token}\n  method: get\n  operationId: getOrderByToken\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders/{order-id}/email-{email}/\n  method: get\n  operationId: getOrderByIdAndEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders/{order-id}/products\n  method: post\n  operationId: addOrderProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/products/{line-number}\n  method: put\n  operationId: updateOrderProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/products/{line-number}\n  method: patch\n  operationId: patchOrderProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/products/{line-number}\n  method: delete\n  operationId: deleteOrderProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/products/{line-number}/sms-ticket-confirmation/{phone-number}\n  method: post\n  operationId: sendTicketConfirmationSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/payments\n  method: post\n  operationId: addOrderPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v3/orders/{order-id}/payments/{line-number}\n  method: delete\n  operationId: deleteOrderPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/refresh-expiration\n  method: post\n  operationId: refreshOrderExpiration\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/loyalty-rewards-application\n  method: post\n  operationId: applyLoyaltyRewards\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/loyalty-rewards-application\n  method: delete\n  operationId: removeLoyaltyRewards\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{order-id}/failed-payment-auths\n  method: post\n  operationId: recordFailedPaymentAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/amc-accounts/{account-id}/orders/\n  method: get\n  operationId: listAccountOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/theatres/{theatre-id}/concessions\n  method: get\n  operationId: listTheatreConcessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/theatres/{theatre-id}/concessions/{concession-id}\n  method: get\n  operationId: getConcession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/concessions/{theatre-product-assignment-id}\n\
  \  method: get\n  operationId: getConcessionByAssignment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/theatres/{theatre-id}/concessions/categories\n  method: get\n  operationId: listConcessionCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/theatres/{theatre-id}/concessions/delivery-locations/{year}/{month}/{day}\n  method: get\n  operationId: listConcessionDeliveryLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/theatres/{theatre-id}/concessions/pickup-times/{year}/{month}/{day}\n  method: get\n  operationId: listConcessionPickupTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/showtimes/{id}/concession-delivery-times\n  method: get\n  operationId: listShowtimeConcessionDeliveryTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/showtimes/{showtime-id}/concession-pickup-times\n  method: get\n  operationId: listShowtimeConcessionPickupTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/loyalty-accounts/{loyalty-account-id}\n  method: get\n  operationId: getLoyaltyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/loyalty-accounts/email-{email-address}\n  method: get\n  operationId: getLoyaltyAccountByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/loyalty-accounts/email-{email-address}/{campaign}/registration\n  method: post\n  operationId: registerLoyaltyByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/loyalty-accounts/card-{card-number}\n  method: get\n  operationId: getLoyaltyAccountByCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/loyalty-accounts/card-{card-number}/{campaign}/registration\n  method: post\n  operationId: registerLoyaltyByCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/loyalty-accounts/phone-{phone}\n  method: get\n  operationId: getLoyaltyAccountByPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/amc-accounts/{amc-account-id}/loyalty\n  method: delete\n  operationId: unlinkLoyaltyAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/loyalty-cards/{card-number}\n  method: get\n  operationId: getLoyaltyCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v4/loyalty-accounts/{loyalty-account-id}/redemptions\n  method: post\n  operationId: createLoyaltyRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/amc-accounts/{account-id}/wallet/views/on-demand\n  method: get\n  operationId: getExternalWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/qr-codes/{encrypted-reference-id}\n  method: get\n  operationId: getTicketQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/code128/{encrypted-reference-id}\n  method: get\n  operationId: getTicketCode128Barcode\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/amc-accounts/{account-id}/loyalty/qr-code\n  method: get\n  operationId: getLoyaltyQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/movies/{movie-id}/confirmation-check/{confirmation-code}\n  method: get\n  operationId: getMovieConfirmationCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fee-waiver\n  method: post\n  operationId: getFeeWaiver\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/webhook-events\n  method: get\n  operationId: listWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook-token-id}\n  method: delete\n  operationId: unsubscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook-token-id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/agentic-access/amc-entertainment-holdings-agentic-access.yml
summary_line: 79 operations · 23 acting
tags:
- Entertainment
- Movies
- Theatres
- Showtimes
- Ticketing
- Concessions
- Loyalty
- Fortune 500
---
