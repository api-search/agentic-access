---
acting_count: 54
action_class_counts:
  acting: 54
  connected: 81
api_specs:
- filename: brushfire-accounts-api-openapi.yml
  format: yaml
  label: Brushfire Accounts API
  slug: brushfire-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-accounts-api-openapi.yml
- filename: brushfire-attendees-api-openapi.yml
  format: yaml
  label: Brushfire Attendees API
  slug: brushfire-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-attendees-api-openapi.yml
- filename: brushfire-cart-api-openapi.yml
  format: yaml
  label: Brushfire Cart API
  slug: brushfire-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-cart-api-openapi.yml
- filename: brushfire-clients-api-openapi.yml
  format: yaml
  label: Brushfire Clients API
  slug: brushfire-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-clients-api-openapi.yml
- filename: brushfire-data-api-openapi.yml
  format: yaml
  label: Brushfire Data API
  slug: brushfire-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-data-api-openapi.yml
- filename: brushfire-events-api-openapi.yml
  format: yaml
  label: Brushfire Events API
  slug: brushfire-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-events-api-openapi.yml
- filename: brushfire-exchanges-api-openapi.yml
  format: yaml
  label: Brushfire Exchanges API
  slug: brushfire-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-exchanges-api-openapi.yml
- filename: brushfire-groups-api-openapi.yml
  format: yaml
  label: Brushfire Groups API
  slug: brushfire-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-groups-api-openapi.yml
- filename: brushfire-hooks-api-openapi.yml
  format: yaml
  label: Brushfire Hooks API
  slug: brushfire-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-hooks-api-openapi.yml
- filename: brushfire-lookups-api-openapi.yml
  format: yaml
  label: Brushfire Lookups API
  slug: brushfire-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-lookups-api-openapi.yml
- filename: brushfire-orders-api-openapi.yml
  format: yaml
  label: Brushfire Orders API
  slug: brushfire-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-orders-api-openapi.yml
- filename: brushfire-paymentprofiles-api-openapi.yml
  format: yaml
  label: Brushfire PaymentProfiles API
  slug: brushfire-paymentprofiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-paymentprofiles-api-openapi.yml
- filename: brushfire-promotions-api-openapi.yml
  format: yaml
  label: Brushfire Promotions API
  slug: brushfire-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-promotions-api-openapi.yml
- filename: brushfire-regions-api-openapi.yml
  format: yaml
  label: Brushfire Regions API
  slug: brushfire-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-regions-api-openapi.yml
- filename: brushfire-sessions-api-openapi.yml
  format: yaml
  label: Brushfire Sessions API
  slug: brushfire-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-sessions-api-openapi.yml
- filename: brushfire-access-codes-api-openapi.yml
  format: yaml
  label: Brushfire Access Codes API
  slug: brushfire-access-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-access-codes-api-openapi.yml
consequence_counts:
  physical: 10
  read: 81
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brushfire Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/pos
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/reader/start
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/fields
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentprofiles/{paymentProfileId}/terminals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sessions/{sessionId}/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sessions/{sessionId}/flex/checkout
operation_count: 135
overview: 'Brushfire exposes 135 API operations that an AI agent could call, of which 54 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 81 read, 44 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brushfire
provider_slug: brushfire
slug: brushfire-agentic-access
source_filename: brushfire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/brushfire-access-codes-api-openapi.yml, openapi/brushfire-accounts-api-openapi.yml,\n  openapi/brushfire-attendees-api-openapi.yml, openapi/brushfire-cart-api-openapi.yml, openapi/brushfire-clients-api-openapi.yml,\n  openapi/brushfire-data-api-openapi.yml, openapi/brushfire-events-api-openapi.yml, openapi/brushfire-exchanges-api-openapi.yml,\n  openapi/brushfire-groups-api-openapi.yml, openapi/brushfire-hooks-api-openapi.yml, openapi/brushfire-lookups-api-openapi.yml,\n  openapi/brushfire-orders-api-openapi.yml, openapi/brushfire-paymentprofiles-api-openapi.yml,\n  openapi/brushfire-promotions-api-openapi.yml, openapi/brushfire-regions-api-openapi.yml, openapi/brushfire-sessions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See\
  \ research/curity/agentic-governance/.\nsummary:\n  operations: 135\n  by_action_class:\n    connected: 81\n    acting: 54\n  by_consequence:\n    read: 81\n    write: 44\n    physical: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /accesscodes\n  method: get\n  operationId: getAccesscodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accesscodes/{accessCodeId}\n  method: get\n  operationId: getAccesscodesByAccessCodeId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accesscodes/dynamic\n  method: post\n  operationId: postAccesscodesDynamic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccountsByAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/auth\n  method: post\n  operationId: postAccountsAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/helpdesk/{email}\n  method: get\n  operationId: getAccountsHelpdeskByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}\n  method: get\n  operationId: getAttendeesByAttendeeId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}/cancel\n  method: post\n  operationId: postAttendeesByAttendeeIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/code\n  method: post\n  operationId: postAttendeesByAttendeeIdCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/communities\n  method: get\n  operationId: getAttendeesByAttendeeIdCommunities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}/community\n  method: post\n  operationId: postAttendeesByAttendeeIdCommunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/completed\n  method: post\n  operationId: postAttendeesByAttendeeIdCompleted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/data\n  method: get\n  operationId: getAttendeesByAttendeeIdData\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}/donate\n  method: post\n  operationId: postAttendeesByAttendeeIdDonate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/fields\n  method: get\n  operationId: getAttendeesByAttendeeIdFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}/fields\n  method: post\n  operationId: postAttendeesByAttendeeIdFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/fieldscustom\n  method: get\n  operationId: getAttendeesByAttendeeIdFieldscustom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}/fieldscustom\n  method: post\n  operationId: postAttendeesByAttendeeIdFieldscustom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/gift\n  method: post\n  operationId: postAttendeesByAttendeeIdGift\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/group\n  method: post\n  operationId: postAttendeesByAttendeeIdGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/link\n  method: post\n  operationId: postAttendeesByAttendeeIdLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/{attendeeId}/print\n  method: get\n  operationId:\
  \ getAttendeesByAttendeeIdPrint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/{attendeeId}/type\n  method: post\n  operationId: postAttendeesByAttendeeIdType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/helpdesk/{email}\n  method: get\n  operationId: getAttendeesHelpdeskByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attendees/ids\n  method: post\n  operationId: postAttendeesIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attendees/print\n  method: post\n  operationId: postAttendeesPrint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}\n  method: get\n  operationId: getCartByCartId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}/events/{eventId}\n  method: delete\n  operationId: deleteCartByCartIdEventsByEventId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/events/{eventId}\n\
  \  method: get\n  operationId: getCartByCartIdEventsByEventId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}/events/{eventId}\n  method: post\n  operationId: postCartByCartIdEventsByEventId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/events/{eventId}/attendees\n  method: post\n  operationId: postCartByCartIdEventsByEventIdAttendees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /cart/{cartId}/events/{eventId}/attendees/{attendeeId}\n  method: delete\n  operationId: deleteCartByCartIdEventsByEventIdAttendeesByAttendeeId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/events/{eventId}/attendees/{attendeeId}\n  method: get\n  operationId: getCartByCartIdEventsByEventIdAttendeesByAttendeeId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}/events/{eventId}/attendees/{attendeeId}\n  method: post\n  operationId: postCartByCartIdEventsByEventIdAttendeesByAttendeeId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/events/{eventId}/attendees/{attendeeId}/form\n  method: get\n  operationId: getCartByCartIdEventsByEventIdAttendeesByAttendeeIdForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}/events/{eventId}/attendees/{attendeeId}/form\n  method: post\n  operationId: postCartByCartIdEventsByEventIdAttendeesByAttendeeIdForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/events/{eventId}/form\n  method: get\n  operationId: getCartByCartIdEventsByEventIdForm\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}/events/{eventId}/form\n  method: post\n  operationId: postCartByCartIdEventsByEventIdForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/events/{eventId}/forms\n  method: get\n  operationId: getCartByCartIdEventsByEventIdForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cartId}/lookup\n  method: get\n  operationId: getCartByCartIdLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cart/{cartId}/promotions\n  method: post\n  operationId: postCartByCartIdPromotions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cartId}/promotions/{promotionId}\n  method: delete\n  operationId: deleteCartByCartIdPromotionsByPromotionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/id\n  method: get\n  operationId: getCartId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n\
  \  method: get\n  operationId: getClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{clientId}\n  method: get\n  operationId: getClientsByClientId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{clientId}/theme\n  method: get\n  operationId: getClientsByClientIdTheme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{id}\n  method: get\n  operationId: getDataById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: post\n  operationId: postEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventId}\n  method: delete\n  operationId: deleteEventsByEventId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventId}\n  method: get\n  operationId: getEventsByEventId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/archive\n\
  \  method: post\n  operationId: postEventsByEventIdArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventId}/bestseats\n  method: get\n  operationId: getEventsByEventIdBestseats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/communities\n  method: get\n  operationId: getEventsByEventIdCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/data\n  method: get\n  operationId: getEventsByEventIdData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/details\n  method: get\n  operationId: getEventsByEventIdDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/documents\n  method: get\n  operationId: getEventsByEventIdDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/fieldmetadata\n  method: get\n  operationId: getEventsByEventIdFieldmetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/fields\n  method: get\n  operationId: getEventsByEventIdFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /events/{eventId}/fields/{fieldId}/remotevalidate\n  method: get\n  operationId: getEventsByEventIdFieldsByFieldIdRemotevalidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/groups\n  method: get\n  operationId: getEventsByEventIdGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/lookup\n  method: get\n  operationId: getEventsByEventIdLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/move\n  method: post\n  operationId: postEventsByEventIdMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventId}/orders\n  method: get\n  operationId: getEventsByEventIdOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/paymentmethods\n  method: get\n  operationId: getEventsByEventIdPaymentmethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/reports/{reportId}\n  method: get\n  operationId: getEventsByEventIdReportsByReportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/resources\n  method: get\n  operationId: getEventsByEventIdResources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/restore\n  method: post\n  operationId: postEventsByEventIdRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventId}/sections\n  method: get\n  operationId: getEventsByEventIdSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/sections/{sectionId}\n  method: get\n  operationId: getEventsByEventIdSectionsBySectionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /events/{eventId}/sections/{sectionId}/seats\n  method: get\n  operationId: getEventsByEventIdSectionsBySectionIdSeats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/sessions\n  method: get\n  operationId: getEventsByEventIdSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/theme\n  method: get\n  operationId: getEventsByEventIdTheme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/types\n  method: get\n  operationId: getEventsByEventIdTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventNumber}/fields/{fieldId}/remotefetch\n\
  \  method: get\n  operationId: getEventsByEventNumberFieldsByFieldIdRemotefetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/copy\n  method: post\n  operationId: postEventsCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchanges\n  method: post\n  operationId: postExchanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchanges/{exchangeId}\n  method: delete\n  operationId: deleteExchangesByExchangeId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchanges/{exchangeId}\n  method: get\n  operationId: getExchangesByExchangeId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges/{exchangeId}\n  method: put\n  operationId: putExchangesByExchangeId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: post\n  operationId: postGroups\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: put\n  operationId: putGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}\n  method: get\n  operationId: getGroupsByGroupId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}/community\n  method: post\n  operationId: postGroupsByGroupIdCommunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/fields\n  method: get\n  operationId: getGroupsByGroupIdFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}/fields\n  method: post\n  operationId: postGroupsByGroupIdFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/print\n  method: get\n  operationId: getGroupsByGroupIdPrint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/helpdesk/{email}\n\
  \  method: get\n  operationId: getGroupsHelpdeskByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/print\n  method: post\n  operationId: postGroupsPrint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hooks/list\n  method: get\n  operationId: getHooksList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hooks/ping\n  method: get\n  operationId: getHooksPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hooks/poll\n  method: get\n  operationId: getHooksPoll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /hooks/sample\n  method: get\n  operationId: getHooksSample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hooks/subscribe\n  method: post\n  operationId: postHooksSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hooks/unsubscribe\n  method: post\n  operationId: postHooksUnsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hooks/update\n\
  \  method: put\n  operationId: putHooksUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookups\n  method: post\n  operationId: postLookups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookups/{lookupId}\n  method: get\n  operationId: getLookupsByLookupId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookups/{lookupId}/events/{eventNumber}\n  method: get\n  operationId: getLookupsByLookupIdEventsByEventNumber\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookups/{lookupId}/events/{eventNumber}/attendees\n  method: get\n  operationId: getLookupsByLookupIdEventsByEventNumberAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookups/{lookupId}/events/{eventNumber}/group\n  method: get\n  operationId: getLookupsByLookupIdEventsByEventNumberGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookups/{lookupId}/events/{eventNumber}/orders\n  method: get\n  operationId: getLookupsByLookupIdEventsByEventNumberOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n\
  \  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: postOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrdersByOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/fields\n  method: get\n  operationId: getOrdersByOrderIdFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/fields\n  method: post\n  operationId: postOrdersByOrderIdFields\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/print\n  method: get\n  operationId: getOrdersByOrderIdPrint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/resend\n  method: post\n  operationId: postOrdersByOrderIdResend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/direct\n  method: post\n  operationId: postOrdersDirect\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/helpdesk/{email}\n  method: get\n  operationId: getOrdersHelpdeskByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (38 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/agentic-access/brushfire-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/agentic-access/brushfire-agentic-access.yml
summary_line: 135 operations · 54 acting
tags:
- Event Ticketing
- Registration
- Event
- Ticketing
- Check-in
- Churches
- Payments
---
