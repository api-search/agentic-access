---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: hyperice-storefront-openapi.yml
  format: yaml
  label: Hyperice Storefront JSON API
  slug: hyperice-storefront-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-storefront-openapi.yml
consequence_counts:
  physical: 3
  read: 8
  write: 10
description: 'Recommended x-agentic-access execution contracts for every operation an agent can reach on Hyperice''s perimeter, classified with the Curity Access Intelligence model. This is a governance STARTING POINT authored by API Evangelist, not a Hyperice claim — with one exception: the human-in-the-loop requirement on complete_checkout is Hyperice''s own published rule, quoted below, not our recommendation.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hyperice Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Hyperice exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 10 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hyperice
provider_slug: hyperice
slug: hyperice-agentic-access
source_filename: hyperice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: generated\nsource:\n- mcp/hyperice-mcp.yml\n- openapi/hyperice-storefront-openapi.yml\n- graphql/hyperice-storefront.graphql\n- https://hyperice.com/llms.txt\ndescription: >-\n  Recommended x-agentic-access execution contracts for every operation an agent\n  can reach on Hyperice's perimeter, classified with the Curity Access\n  Intelligence model. This is a governance STARTING POINT authored by API\n  Evangelist, not a Hyperice claim — with one exception: the human-in-the-loop\n  requirement on complete_checkout is Hyperice's own published rule, quoted\n  below, not our recommendation.\nprovider_published_rules:\n- rule: human-in-the-loop on payment\n  quote: >-\n    \"Checkout requires human approval. Agents must not complete payment without\n    explicit buyer consent. If you cannot get contemporaneous buyer approval at\n    the moment of payment, install https://shop.app/SKILL.md and route the\n    purchase through Shop Pay instead.\"\n\
  \  source: https://hyperice.com/llms.txt\n- rule: backoff\n  quote: 'Respect rate limits. The MCP endpoint is rate-limited per IP. Back off on 429 responses.'\n  source: https://hyperice.com/llms.txt\n- rule: buyer context\n  quote: 'Use buyer context. Pass context.address_country and context.currency for accurate pricing and availability.'\n  source: https://hyperice.com/llms.txt\n- rule: agent identity\n  quote: >-\n    The MCP endpoint refuses to enumerate or invoke tools without a resolvable\n    UCP agent profile URI (observed HTTP 422 invalid_profile_url).\n  source: https://hyperice.com/api/ucp/mcp\nsummary:\n  operations: 21\n  by_action_class: {connected: 8, acting: 13}\n  by_consequence: {read: 8, write: 10, physical: 3}\n  human_in_the_loop: 1\n  audit_required: 13\n  audience: null\n  note: >-\n    audience is deliberately left null on every entry — it binds per deployment,\n    not per provider.\noperations:\n- id: listProducts\n  surface: rest\n  action_class: connected\n\
  \  consequence: read\n  scope: 'catalog:read'\n  token: {ttl_max_seconds: 3600, type: none}\n  audit: optional\n- id: getProduct\n  surface: rest\n  action_class: connected\n  consequence: read\n  scope: 'catalog:read'\n  token: {ttl_max_seconds: 3600, type: none}\n  audit: optional\n- id: listCollections\n  surface: rest\n  action_class: connected\n  consequence: read\n  scope: 'catalog:read'\n  token: {ttl_max_seconds: 3600, type: none}\n  audit: optional\n- id: listCollectionProducts\n  surface: rest\n  action_class: connected\n  consequence: read\n  scope: 'catalog:read'\n  token: {ttl_max_seconds: 3600, type: none}\n  audit: optional\n- id: getUcpProfile\n  surface: rest\n  action_class: connected\n  consequence: read\n  scope: 'discovery:read'\n  token: {ttl_max_seconds: 3600, type: none}\n  audit: optional\n- id: getLlmsTxt\n  surface: rest\n  action_class: connected\n  consequence: read\n  scope: 'discovery:read'\n  token: {ttl_max_seconds: 3600, type: none}\n  audit: optional\n\
  - id: search_catalog\n  surface: mcp\n  action_class: connected\n  consequence: read\n  scope: 'catalog:read'\n  token: {ttl_max_seconds: 3600, type: ucp-agent-profile}\n  audit: optional\n- id: lookup_catalog\n  surface: mcp\n  action_class: connected\n  consequence: read\n  scope: 'catalog:read'\n  token: {ttl_max_seconds: 3600, type: ucp-agent-profile}\n  audit: optional\n- id: create_cart\n  surface: mcp\n  action_class: acting\n  consequence: write\n  scope: 'cart:write'\n  token: {ttl_max_seconds: 900, type: ucp-agent-profile}\n  idempotency: \"meta['idempotency-key']\"\n  audit: required\n- id: update_cart\n  surface: mcp\n  action_class: acting\n  consequence: write\n  scope: 'cart:write'\n  token: {ttl_max_seconds: 900, type: ucp-agent-profile}\n  idempotency: \"meta['idempotency-key']\"\n  audit: required\n- id: cancel_cart\n  surface: mcp\n  action_class: acting\n  consequence: write\n  scope: 'cart:write'\n  token: {ttl_max_seconds: 900, type: ucp-agent-profile}\n  idempotency:\
  \ \"meta['idempotency-key']\"\n  audit: required\n- id: create_checkout\n  surface: mcp\n  action_class: acting\n  consequence: write\n  scope: 'checkout:write'\n  token: {ttl_max_seconds: 900, type: ucp-agent-profile}\n  idempotency: \"meta['idempotency-key']\"\n  audit: required\n- id: update_checkout\n  surface: mcp\n  action_class: acting\n  consequence: write\n  scope: 'checkout:write'\n  token: {ttl_max_seconds: 900, type: ucp-agent-profile}\n  idempotency: \"meta['idempotency-key']\"\n  audit: required\n  note: Writes the buyer's physical shipping address — treat the payload as PII.\n- id: cancel_checkout\n  surface: mcp\n  action_class: acting\n  consequence: write\n  scope: 'checkout:write'\n  token: {ttl_max_seconds: 900, type: ucp-agent-profile}\n  audit: required\n- id: complete_checkout\n  surface: mcp\n  action_class: acting\n  consequence: physical\n  scope: 'checkout:complete'\n  token: {ttl_max_seconds: 300, type: ucp-agent-profile, exchange: required, purpose_required:\
  \ true}\n  idempotency: \"meta['idempotency-key']\"\n  human_in_the_loop: required\n  audit: required\n  rationale: >-\n    Charges a real payment instrument and dispatches a physical shipment.\n    Irreversible by the agent. Hyperice itself mandates explicit buyer consent\n    at the moment of payment.\n- id: get_order\n  surface: mcp\n  action_class: connected\n  consequence: read\n  scope: 'customer-account-mcp-api:full'\n  token: {ttl_max_seconds: 900, type: oidc-bearer}\n  audit: required\n  note: >-\n    Reads buyer-owned order data. Classified read, but the only scope Hyperice\n    offers is a :full grant, so least privilege is not achievable here.\n- id: cartSubmitForCompletion\n  surface: graphql\n  action_class: acting\n  consequence: physical\n  scope: 'checkout:complete'\n  token: {ttl_max_seconds: 300, type: none, exchange: required, purpose_required: true}\n  human_in_the_loop: required\n  audit: required\n  rationale: The GraphQL equivalent of complete_checkout. Places a\
  \ real order.\n- id: shopPayPaymentRequestSessionSubmit\n  surface: graphql\n  action_class: acting\n  consequence: physical\n  scope: 'payment:submit'\n  token: {ttl_max_seconds: 300, type: session-token, exchange: required, purpose_required: true}\n  idempotency: 'idempotencyKey (String!, required)'\n  human_in_the_loop: required\n  audit: required\n  rationale: Submits a Shop Pay payment transaction. The only GraphQL mutation with mandatory idempotency.\n- id: customerCreate\n  surface: graphql\n  action_class: acting\n  consequence: write\n  scope: 'customer:write'\n  token: {ttl_max_seconds: 900, type: none}\n  audit: required\n  note: Creates a real customer record from agent-supplied PII. No CAPTCHA or agent gate observed.\n- id: customerUpdate\n  surface: graphql\n  action_class: acting\n  consequence: write\n  scope: 'customer:write'\n  token: {ttl_max_seconds: 900, type: customer-access-token}\n  audit: required\n- id: customerAccessTokenCreate\n  surface: graphql\n  action_class:\
  \ acting\n  consequence: write\n  scope: 'customer:authenticate'\n  token: {ttl_max_seconds: 900, type: none}\n  audit: required\n  note: >-\n    Exchanges buyer email+password for a customer access token on an\n    unauthenticated endpoint. Highest-risk non-payment operation on the\n    perimeter; rate-limit and abuse controls are not published.\ngovernance_observations:\n- >-\n  The single highest-consequence tool (complete_checkout) is the one Hyperice\n  explicitly fences with a human-approval rule — the provider's own guidance and\n  this classification agree.\n- >-\n  The Storefront GraphQL API is served in public access mode, so every cart and\n  customer mutation is reachable with no credential at all. That is the widest\n  agentic exposure on this perimeter and it is entirely undocumented by Hyperice,\n  whose /llms.txt describes only the read-only surface and the UCP tools.\n- >-\n  Scope granularity is the weakest control: the only buyer-scoped grants are\n  customer-account-api:full\
  \ and customer-account-mcp-api:full, so an agent that\n  needs to read an order must be trusted to mutate the profile.\nx-evidence:\n  fetched: '2026-07-31'\n  note: >-\n    Operation inventory is grounded in the live introspected schema, the UCP\n    OpenRPC method list Hyperice's profile designates, and the derived REST\n    OpenAPI. No operation listed here is invented; the access classification\n    itself is our recommendation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/agentic-access/hyperice-agentic-access.yml
summary_line: 21 operations · 13 acting
tags:
- Company
- Commerce
- Retail
- Health and Wellness
- Consumer Hardware
- Sports And Fitness
- Agentic Commerce
- GraphQL
- MCP
- Shopify
---
