---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 6
consequence_counts:
  physical: 2
  read: 6
  write: 8
description: Recommended x-agentic-access execution contracts for the ColdSnap agent surface. ColdSnap publishes no OpenAPI, so operations are the live MCP tools and the GraphQL mutation families they project over, not REST operationIds. A governance starting point — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Coldsnap Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
operation_count: 16
overview: 'ColdSnap exposes 16 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 8 write, and 2 physical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ColdSnap
provider_slug: coldsnap
slug: coldsnap-agentic-access
source_filename: coldsnap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: >-\n  mcp/coldsnap-mcp.yml (live tools/list, 5 tools), graphql/coldsnap-storefront.graphql\n  (live introspection, 41 mutations), https://coldsnap.com/agents.md,\n  https://coldsnap.com/robots.txt\ndescription: >-\n  Recommended x-agentic-access execution contracts for the ColdSnap agent surface. ColdSnap\n  publishes no OpenAPI, so operations are the live MCP tools and the GraphQL mutation\n  families they project over, not REST operationIds. A governance starting point — review\n  and bind audience per deployment. See research/curity/agentic-governance/.\nprovider_stated_policy:\n  source: https://coldsnap.com/robots.txt and https://coldsnap.com/agents.md\n  rule: >-\n    \"Checkouts are for humans. Do NOT complete checkout, payment, or order placement\n    automatically — no scripted form fills, browser automation, or end-to-end agent flows\n    that finalize payment without an explicit, contemporaneous human approval step.\"\
  \n  note: >-\n    This is the rare case where the provider publishes its own agent escalation rule. The\n    human-in-the-loop classification on the payment-adjacent operations below is the\n    provider's stated policy, not our heuristic.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 6\n    acting: 10\n  by_consequence:\n    read: 6\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 2\n  surfaces: [mcp, graphql, json-ajax]\noperations:\n- surface: mcp\n  endpoint: https://coldsnap.com/api/mcp\n  tool: search_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- surface: mcp\n  endpoint: https://coldsnap.com/api/mcp\n  tool: get_product_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- surface: mcp\n  endpoint: https://coldsnap.com/api/mcp\n  tool: get_cart\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    note: >-\n      The opaque cart_id is the bearer of cart identity on an otherwise anonymous surface.\n      Treat it as a secret — anyone holding it can read and mutate that cart.\n- surface: mcp\n  endpoint: https://coldsnap.com/api/mcp\n  tool: search_shop_policies_and_faqs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- surface: mcp\n  endpoint: https://coldsnap.com/api/mcp\n  tool: update_cart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers: [high-value, buyer-identity-change, delivery-address-change]\n    audit: required\n    note: >-\n      A single\
  \ consolidated tool that fans out across eleven GraphQL cart mutations,\n      including buyer_identity and delivery addresses — personal data enters the cart here.\n      No idempotency key is offered, so a naive retry duplicates line items.\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: cart-create-and-lines\n  fields: [cartCreate, cartLinesAdd, cartLinesUpdate, cartLinesRemove]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers: [high-value]\n    audit: required\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: cart-buyer-identity\n  fields: [cartBuyerIdentityUpdate, cartBillingAddressUpdate, cartDeliveryAddressesAdd, cartDeliveryAddressesReplace, cartDeliveryAddressesUpdate, cartDeliveryAddressesRemove]\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    purpose: required\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers: [pii-write]\n    audit: required\n    note: Writes buyer name, email, phone and postal addresses onto the cart.\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: cart-personal-data-erasure\n  fields: [cartRemovePersonalData]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers: [destructive]\n    audit: required\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: cart-discounts-and-gift-cards\n  fields: [cartDiscountCodesUpdate, cartGiftCardCodesAdd, cartGiftCardCodesUpdate, cartGiftCardCodesRemove]\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers: [value-bearing-instrument]\n    audit: required\n    note: Gift-card codes are bearer instruments; do not log them.\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: cart-metadata\n  fields: [cartAttributesUpdate, cartNoteUpdate, cartMetafieldsSet, cartMetafieldDelete, cartClone]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: cart-payment\n  fields: [cartPaymentUpdate]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    purpose: required\n    token:\n      max-ttl:\
  \ 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      triggers: [payment]\n    audit: required\n    note: >-\n      Provider-stated policy. Payment instrument attachment must not happen without\n      contemporaneous buyer approval.\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: checkout-completion\n  fields: [cartPrepareForCompletion, cartSubmitForCompletion, shopPayPaymentRequestSessionCreate, shopPayPaymentRequestSessionSubmit]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    purpose: required\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      triggers: [payment, order-placement]\n    audit: required\n    note: >-\n      Provider-stated policy, verbatim in robots.txt and /agents.md. Agents without\n      contemporaneous approval are directed to route through\
  \ Shop Pay via\n      https://shop.app/SKILL.md instead. Deliberately absent from the anonymous MCP tool set.\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: customer-identity\n  fields: [customerCreate, customerActivate, customerActivateByUrl, customerRecover, customerReset, customerResetByUrl, customerUpdate]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    purpose: required\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers: [account-creation, credential-change]\n    audit: required\n    note: >-\n      Account creation and password reset. Not exposed by any MCP tool; requires a customer\n      access token issued through the Shopify customer-accounts OIDC flow.\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: customer-access-tokens\n  fields: [customerAccessTokenCreate,\
  \ customerAccessTokenCreateWithMultipass, customerAccessTokenRenew, customerAccessTokenDelete]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    purpose: required\n    token:\n      max-ttl: 900\n      exchange: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers: [credential-issuance]\n    audit: required\n- surface: graphql\n  endpoint: https://coldsnap.com/api/2026-07/graphql.json\n  operation_family: customer-addresses\n  fields: [customerAddressCreate, customerAddressUpdate, customerAddressDelete, customerDefaultAddressUpdate]\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    purpose: required\n    token:\n      max-ttl: 900\n    audit: required\n- surface: json-ajax\n  endpoint: https://coldsnap.com/\n  operation_family: read-only-catalog\n  paths:\n  - /products.json\n  - '/products/{handle}.json'\n  - /collections.json\n\
  \  - '/collections/{handle}/products.json'\n  - /cart.js\n  - /search\n  - /sitemap.xml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    note: Unauthenticated, advertised to agents in /agents.md.\nnotes:\n- >-\n  Every field named above was verified present in the live introspected schema at\n  graphql/coldsnap-storefront.graphql; every tool was returned by a live tools/list.\n- >-\n  audience is left null throughout — bind it per deployment.\n- >-\n  The UCP endpoint at /api/ucp/mcp could not be enumerated anonymously (422 /\n  invalid_profile_url), so its tool-level contracts are not classified here.\nx-evidence:\n  generated_from:\n  - mcp/coldsnap-mcp.yml\n  - graphql/coldsnap-storefront.graphql\n  - https://coldsnap.com/agents.md\n  - https://coldsnap.com/robots.txt\n  date: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coldsnap/refs/heads/main/agentic-access/coldsnap-agentic-access.yml
summary_line: 16 operations · 10 acting · 2 human-in-the-loop
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Food and Beverage
- Consumer Products
- Hardware
- Appliances
- Food Service
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
