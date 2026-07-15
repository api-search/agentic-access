---
acting_count: 67
action_class_counts:
  acting: 67
  connected: 52
api_specs:
- filename: godaddy-domains-openapi.json
  format: json
  label: GoDaddy Domains API
  slug: domains
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-domains-openapi.json
- filename: godaddy-certificates-openapi.json
  format: json
  label: GoDaddy Certificates API
  slug: certificates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-certificates-openapi.json
- filename: godaddy-shoppers-openapi.json
  format: json
  label: GoDaddy Shoppers API
  slug: shoppers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-shoppers-openapi.json
- filename: godaddy-subscriptions-openapi.json
  format: json
  label: GoDaddy Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-subscriptions-openapi.json
- filename: godaddy-orders-openapi.json
  format: json
  label: GoDaddy Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-orders-openapi.json
- filename: godaddy-aftermarket-openapi.json
  format: json
  label: GoDaddy Aftermarket API
  slug: aftermarket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-aftermarket-openapi.json
- filename: godaddy-abuse-openapi.json
  format: json
  label: GoDaddy Abuse API
  slug: abuse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-abuse-openapi.json
- filename: godaddy-agreements-openapi.json
  format: json
  label: GoDaddy Agreements API
  slug: agreements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-agreements-openapi.json
- filename: godaddy-countries-openapi.json
  format: json
  label: GoDaddy Countries API
  slug: countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-countries-openapi.json
consequence_counts:
  physical: 24
  read: 52
  safety-critical: 2
  write: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Godaddy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/certificates/{certificateId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/certificates/{certificateId}/verifyDomainControl
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/certificates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/certificates/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/certificates/{certificateId}/email/resend/{emailAddress}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/certificates/{certificateId}/email/{emailId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/certificates/{certificateId}/email/{emailId}/resend/{emailAddress}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains/available
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains/purchase/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains/{domain}/privacy/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains/{domain}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domains/{domain}/verifyRegistrantEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/certificates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/register
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/redeem
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transfer/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transferInAccept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transferInCancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transferInRestart
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transferInRetry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transferOut
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/customers/{customerId}/domains/{domain}/transferOutAccept
operation_count: 119
overview: 'GoDaddy exposes 119 API operations that an AI agent could call, of which 67 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 52 read, 41 write, 24 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoDaddy
provider_slug: godaddy
slug: godaddy-agentic-access
source_filename: godaddy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/godaddy-abuse-openapi.json, openapi/godaddy-aftermarket-openapi.json, openapi/godaddy-agreements-openapi.json,\n  openapi/godaddy-certificates-openapi.json, openapi/godaddy-countries-openapi.json, openapi/godaddy-domains-openapi.json,\n  openapi/godaddy-orders-openapi.json, openapi/godaddy-shoppers-openapi.json, openapi/godaddy-subscriptions-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 119\n  by_action_class:\n    connected: 52\n    acting: 67\n  by_consequence:\n    read: 52\n    write: 41\n    physical: 24\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/abuse/tickets\n  method: get\n  operationId: getTickets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/abuse/tickets\n  method: post\n  operationId: createTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/abuse/tickets/{ticketId}\n  method: get\n  operationId: getTicketInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/abuse/tickets\n  method: get\n  operationId: getTicketsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/abuse/tickets\n  method: post\n  operationId: createTicketV2\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/abuse/tickets/{ticketId}\n  method: get\n  operationId: getTicketInfoV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customerId}/auctions/listings\n  method: get\n  operationId: getListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aftermarket/listings\n  method: delete\n  operationId: deleteListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aftermarket/listings/expiry\n  method: post\n  operationId: addExpiryListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agreements\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates\n  method: post\n  operationId: certificate_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/validate\n  method: post\n  operationId: certificate_validate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}\n  method: get\n  operationId: certificate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{certificateId}/actions\n  method: get\n  operationId: certificate_action_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{certificateId}/email/{emailId}/resend\n\
  \  method: post\n  operationId: certificate_resend_email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/email/resend/{emailAddress}\n  method: post\n  operationId: certificate_alternate_email_address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/email/{emailId}/resend/{emailAddress}\n  method: post\n  operationId: certificate_resend_email_address\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/email/history\n  method: get\n  operationId: certificate_email_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{certificateId}/callback\n  method: delete\n  operationId: certificate_callback_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/callback\n\
  \  method: get\n  operationId: certificate_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{certificateId}/callback\n  method: put\n  operationId: certificate_callback_replace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/cancel\n  method: post\n  operationId: certificate_cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/download\n\
  \  method: get\n  operationId: certificate_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{certificateId}/reissue\n  method: post\n  operationId: certificate_reissue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/renew\n  method: post\n  operationId: certificate_renew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates/{certificateId}/revoke\n\
  \  method: post\n  operationId: certificate_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/certificates/{certificateId}/siteSeal\n  method: get\n  operationId: certificate_siteseal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{certificateId}/verifyDomainControl\n  method: post\n  operationId: certificate_verifydomaincontrol\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v2/certificates\n  method: get\n  operationId: certificate_get_entitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/certificates\n  method: post\n  operationId: certificate_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/certificates/{certificateId}/reissue\n  method: post\n  operationId: certificate_reissue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/certificates/download\n  method: get\n  operationId: certificate_download_entitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/certificates\n  method: get\n  operationId: getCustomerCertificatesByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/certificates/{certificateId}\n  method: get\n  operationId: getCertificateDetailByCertIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/certificates/{certificateId}/domainVerifications\n  method: get\n  operationId: getDomainInformationByCertificateId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/certificates/{certificateId}/domainVerifications/{domain}\n  method: get\n  operationId: getDomainDetailsByDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/certificates/acme/externalAccountBinding\n  method: get\n  operationId: getAcmeExternalAccountBinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/certificates/subscriptions/search\n  method: get\n  operationId: retrieveSslByDomainReseller\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/certificates/subscription/{guid}\n\
  \  method: get\n  operationId: retrieveSslByDomainSubscriptionReseller\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{countryKey}\n  method: get\n  operationId: getCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n  method: get\n  operationId: list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/agreements\n  method: get\n  operationId: getAgreement\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/available\n  method: get\n  operationId: available\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/available\n  method: post\n  operationId: availableBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/contacts/validate\n  method: post\n  operationId: ContactsValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/purchase\n  method: post\n  operationId: purchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/purchase/schema/{tld}\n  method: get\n  operationId: schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/purchase/validate\n  method: post\n  operationId: validate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/suggest\n  method: get\n  operationId: suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/tlds\n  method: get\n  operationId: tlds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}\n  method: delete\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}\n  method: get\n  operationId:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}\n  method: patch\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/contacts\n  method: patch\n  operationId: updateContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/privacy\n  method: delete\n  operationId: cancelPrivacy\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/privacy/purchase\n  method: post\n  operationId: purchasePrivacy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/records\n  method: patch\n  operationId: recordAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/domains/{domain}/records\n  method: put\n  operationId: recordReplace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/records/{type}/{name}\n  method: get\n  operationId: recordGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/records/{type}/{name}\n  method: put\n  operationId: recordReplaceTypeName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/domains/{domain}/records/{type}/{name}\n  method: delete\n  operationId: recordDeleteTypeName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/records/{type}\n  method: put\n  operationId: recordReplaceType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/renew\n  method: post\n  operationId: renew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/transfer\n  method: post\n  operationId: transferIn\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}/verifyRegistrantEmail\n  method: post\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/{domain}/changeOfRegistrant\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/changeOfRegistrant\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/{domain}/dnssecRecords\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/dnssecRecords\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/nameServers\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/privacy/forwarding\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/{domain}/privacy/forwarding\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/redeem\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/renew\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transfer\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transfer\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/{domain}/transfer/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferInAccept\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferInCancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferInRestart\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferInRetry\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferOut\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferOutAccept\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/transferOutReject\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/forwards/{fqdn}\n  method: delete\n  operationId: domainsForwardsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/forwards/{fqdn}\n  method: get\n  operationId: domainsForwardsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/forwards/{fqdn}\n  method: put\n  operationId: domainsForwardsPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/forwards/{fqdn}\n  method: post\n  operationId: domainsForwardsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/actions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/{domain}/actions/{type}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/{domain}/actions/{type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/notifications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/notifications/optIn\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/notifications/optIn\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/notifications/schemas/{type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/notifications/{notificationId}/acknowledge\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/register\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers/{customerId}/domains/register/schema/{tld}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers/{customerId}/domains/register/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/domains/maintenances\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/domains/maintenances/{ma\n\n\
  # --- truncated at 32 KB (36 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/agentic-access/godaddy-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/agentic-access/godaddy-agentic-access.yml
summary_line: 119 operations · 67 acting · 2 human-in-the-loop
tags:
- Aftermarket
- Certificates
- DNS
- Domains
- Hosting
- Registrar
---
