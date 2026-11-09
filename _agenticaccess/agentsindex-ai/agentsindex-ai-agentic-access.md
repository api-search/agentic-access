---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 18
api_specs:
- filename: agentsindex-ai-agent-api-openapi.yml
  format: yaml
  label: AgentsIndex Agent API
  slug: agentsindex-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-agent-api-openapi.yml
- filename: agentsindex-ai-agentsindex-machine-api-api-openapi.yml
  format: yaml
  label: AgentsIndex AgentsIndex — Machine API
  slug: agentsindex-ai-agentsindex-machine-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-agentsindex-machine-api-api-openapi.yml
- filename: agentsindex-ai-blog-api-openapi.yml
  format: yaml
  label: AgentsIndex Blog API
  slug: agentsindex-ai-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-blog-api-openapi.yml
- filename: agentsindex-ai-blog-md-api-openapi.yml
  format: yaml
  label: AgentsIndex Blog.md API
  slug: agentsindex-ai-blog-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-blog-md-api-openapi.yml
- filename: agentsindex-ai-categories-api-openapi.yml
  format: yaml
  label: AgentsIndex Categories API
  slug: agentsindex-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-categories-api-openapi.yml
- filename: agentsindex-ai-domain-proof-api-openapi.yml
  format: yaml
  label: AgentsIndex Domain Proof API
  slug: agentsindex-ai-domain-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-domain-proof-api-openapi.yml
- filename: agentsindex-ai-guides-api-openapi.yml
  format: yaml
  label: AgentsIndex Guides API
  slug: agentsindex-ai-guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-guides-api-openapi.yml
- filename: agentsindex-ai-index-json-api-openapi.yml
  format: yaml
  label: AgentsIndex Index.json API
  slug: agentsindex-ai-index-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-index-json-api-openapi.yml
- filename: agentsindex-ai-lead-api-openapi.yml
  format: yaml
  label: AgentsIndex Lead API
  slug: agentsindex-ai-lead-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-lead-api-openapi.yml
- filename: agentsindex-ai-listings-json-api-openapi.yml
  format: yaml
  label: AgentsIndex Listings.json API
  slug: agentsindex-ai-listings-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-listings-json-api-openapi.yml
- filename: agentsindex-ai-llms-full-txt-api-openapi.yml
  format: yaml
  label: AgentsIndex Llms Full.txt API
  slug: agentsindex-ai-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-llms-full-txt-api-openapi.yml
- filename: agentsindex-ai-llms-txt-api-openapi.yml
  format: yaml
  label: AgentsIndex Llms.txt API
  slug: agentsindex-ai-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-llms-txt-api-openapi.yml
- filename: agentsindex-ai-mcp-api-openapi.yml
  format: yaml
  label: AgentsIndex MCP API
  slug: agentsindex-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-mcp-api-openapi.yml
- filename: agentsindex-ai-methodology-md-api-openapi.yml
  format: yaml
  label: AgentsIndex Methodology.md API
  slug: agentsindex-ai-methodology-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-methodology-md-api-openapi.yml
- filename: agentsindex-ai-newsletter-api-openapi.yml
  format: yaml
  label: AgentsIndex Newsletter API
  slug: agentsindex-ai-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-newsletter-api-openapi.yml
- filename: agentsindex-ai-owner-api-openapi.yml
  format: yaml
  label: AgentsIndex Owner API
  slug: agentsindex-ai-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-owner-api-openapi.yml
- filename: agentsindex-ai-search-api-openapi.yml
  format: yaml
  label: AgentsIndex Search API
  slug: agentsindex-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-search-api-openapi.yml
- filename: agentsindex-ai-submissions-api-openapi.yml
  format: yaml
  label: AgentsIndex Submissions API
  slug: agentsindex-ai-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-submissions-api-openapi.yml
- filename: agentsindex-ai-submit-api-openapi.yml
  format: yaml
  label: AgentsIndex Submit API
  slug: agentsindex-ai-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-submit-api-openapi.yml
consequence_counts:
  physical: 3
  read: 18
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentsindex Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agent/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agent/orders/{id}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lead
operation_count: 26
overview: 'AgentsIndex exposes 26 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 5 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentsIndex
provider_slug: agentsindex-ai
slug: agentsindex-ai-agentic-access
source_filename: agentsindex-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentsindex-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 18\n    acting: 8\n  by_consequence:\n    read: 18\n    write: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/search\n  method: get\n  operationId: searchListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings.json\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{slug}.md\n\
  \  method: get\n  operationId: getListingMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{slug}.md\n  method: get\n  operationId: getCategoryMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{slug}.json\n  method: get\n  operationId: getCategoryExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /guides/{slug}.md\n  method: get\n  operationId: getGuideMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog.md\n  method: get\n  operationId: getBlogIndexMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog/{slug}.md\n  method: get\n  operationId: getBlogPostMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /methodology.md\n  method: get\n  operationId: getMethodologyMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index.json\n  method: get\n  operationId:\
  \ getMachineManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/submit\n  method: post\n  operationId: submitListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domain-proof/start\n  method: post\n  operationId: startDomainProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domain-proof/verify\n  method: post\n  operationId: verifyDomainProof\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/submissions/{id}\n  method: get\n  operationId: getSubmissionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lead\n  method: post\n  operationId: submitLead\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/newsletter/subscribe\n  method: post\n  operationId: subscribeNewsletter\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/owner/listings\n  method: get\n  operationId: getOwnerListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/catalogue\n  method: get\n  operationId: getAgentCatalogue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/quotes\n\
  \  method: post\n  operationId: getAgentQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/orders\n  method: post\n  operationId: createAgentOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/orders/{id}\n  method: get\n  operationId: getAgentOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/orders/{id}/payment\n  method: post\n  operationId: payAgentOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/orders/{id}/receipt\n  method: get\n  operationId: getAgentOrderReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentsindex-ai/agentic-access/agentsindex-ai-agentic-access.yml
summary_line: 26 operations · 8 acting
tags:
- Artificial Intelligence
- Index
- Tools
- Catalog
- Agents
- Marketplace
---
