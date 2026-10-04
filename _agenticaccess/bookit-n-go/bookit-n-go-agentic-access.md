---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 16
api_specs:
- filename: bookit-n-go-agent-api-openapi.yml
  format: yaml
  label: Bookit N Go Agent API
  slug: bookit-n-go-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-agent-api-openapi.yml
- filename: bookit-n-go-flights-api-openapi.yml
  format: yaml
  label: Bookit N Go Flights API
  slug: bookit-n-go-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-flights-api-openapi.yml
- filename: bookit-n-go-hotels-api-openapi.yml
  format: yaml
  label: Bookit N Go Hotels API
  slug: bookit-n-go-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-hotels-api-openapi.yml
- filename: bookit-n-go-travelers-api-openapi.yml
  format: yaml
  label: Bookit N Go Travelers API
  slug: bookit-n-go-travelers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-travelers-api-openapi.yml
- filename: bookit-n-go-trips-api-openapi.yml
  format: yaml
  label: Bookit N Go Trips API
  slug: bookit-n-go-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-trips-api-openapi.yml
- filename: bookit-n-go-webhooks-api-openapi.yml
  format: yaml
  label: Bookit N Go Webhooks API
  slug: bookit-n-go-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-webhooks-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 1
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Bookit N Go Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /travelers/profiles/{profileId}/consents/{consentId}/revoke
operation_count: 37
overview: 'Bookit N Go exposes 37 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 20 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bookit N Go
provider_slug: bookit-n-go
slug: bookit-n-go-agentic-access
source_filename: bookit-n-go-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/bookit-n-go-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 21\n    connected: 16\n  by_consequence:\n    write: 20\n    read: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /travelers/profiles\n  method: post\n  operationId: publicCreateTravelerProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travelers/profiles/{profileId}\n  method: get\n  operationId: publicGetTravelerProfile\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travelers/profiles/{profileId}\n  method: patch\n  operationId: publicUpdateTravelerProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travelers/profiles/{profileId}/preferences\n  method: get\n  operationId: publicListTravelerPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travelers/profiles/{profileId}/preferences\n  method: put\n  operationId: publicReplaceTravelerPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travelers/profiles/{profileId}/constraints\n  method: get\n  operationId: publicListTravelerConstraints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travelers/profiles/{profileId}/constraints\n  method: put\n  operationId: publicReplaceTravelerConstraints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travelers/profiles/{profileId}/consents\n  method: get\n  operationId: publicListTravelerConsents\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travelers/profiles/{profileId}/consents\n  method: post\n  operationId: publicGrantTravelerConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travelers/profiles/{profileId}/consents/{consentId}/revoke\n  method: post\n  operationId: publicRevokeTravelerConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent/actions/prepare\n  method: post\n  operationId: publicPrepareAgentAction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/actions/{receiptId}/execute\n  method: post\n  operationId: publicExecuteAgentAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/receipts/{receiptId}\n  method: get\n  operationId: publicGetAgentReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: get\n  operationId: publicListTrips\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: post\n  operationId: publicCreateTrip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trips/{tripId}\n  method: get\n  operationId: publicGetTrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{tripId}/items\n  method: post\n  operationId: publicAddTripItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /trips/{tripId}/items/{itemId}/servicing/cancellation-preview\n  method: post\n  operationId: publicCreateCancellationPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trips/{tripId}/items/{itemId}/servicing/cancel\n  method: post\n  operationId: publicCancelTripItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trips/{tripId}/servicing/actions/{actionId}\n  method: get\n  operationId: publicGetServicingAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: publicCreateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: publicListWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: publicDeleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}/rotate-secret\n\
  \  method: post\n  operationId: publicRotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}/deliveries\n  method: get\n  operationId: publicListWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/search\n  method: post\n  operationId: publicSearchFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommendations/flights\n  method: post\n  operationId: publicRankFlights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recommendations/hotels\n  method: post\n  operationId: publicRankHotels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recommendations/receipts/{receiptId}\n  method: get\n  operationId: publicGetRecommendationReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/{offerId}/revalidate\n  method: post\n  operationId: publicRevalidateFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flights/{offerId}/fare-rules\n  method: get\n  operationId: publicGetFlightFareRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/bookings\n  method: post\n  operationId: publicCreateFlightBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flights/bookings/{bookingId}\n  method: get\n  operationId: publicGetFlightBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /hotels/search\n  method: post\n  operationId: publicSearchHotels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotels/{offerId}/revalidate\n  method: post\n  operationId: publicRevalidateHotel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotels/bookings\n  method: post\n  operationId: publicCreateHotelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotels/bookings/{bookingId}\n  method: get\n  operationId:\
  \ publicGetHotelBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/agentic-access/bookit-n-go-agentic-access.yml
summary_line: 37 operations · 21 acting · 1 human-in-the-loop
tags:
- Travel
- SaaS
- AI
- White-label
- B2B
---
