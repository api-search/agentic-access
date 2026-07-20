---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 22
api_specs:
- filename: docs
  format: yaml
  label: Craft.io Workspace API
  slug: craftio-workspace-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
- filename: docs
  format: yaml
  label: Craft.io Portfolio API
  slug: craftio-portfolio-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
- filename: docs
  format: yaml
  label: Craft.io Feedback Portal API
  slug: craftio-feedback-portal-api
  spec_type: OpenAPI
  url: https://api.craft.io/docs
consequence_counts:
  read: 22
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Craft Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Craft.io exposes 27 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Craft.io
provider_slug: craft-io
slug: craft-io-agentic-access
source_filename: craft-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/craft-io-feedback-openapi.yml, openapi/craft-io-portfolio-openapi.yml, openapi/craft-io-workspace-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 22\n    acting: 5\n  by_consequence:\n    read: 22\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /feedback_portals/{accountId}\n  method: get\n  operationId: GetPortals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_portals\n  method: get\n  operationId: GetPortalsExtended\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_portal/{portalId}/categories\n  method: get\n  operationId: GetCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_portal/{portalId}/importances\n  method: get\n  operationId: GetImportances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_portal/{portalId}/feedback_items\n  method: get\n  operationId: GetIdeas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_item/{ideaId}\n\
  \  method: get\n  operationId: GetIdea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_portal/{portalId}/plain_feedback\n  method: post\n  operationId: PostPlainIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:feedback:craft\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback_portal/{portalId}/feedback\n  method: post\n  operationId: PostIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:feedback:craft\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /feedback_portal/{portalId}/custom_fields\n  method: get\n  operationId: GetCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback_portal/{portalId}/forms\n  method: get\n  operationId: GetForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:feedback:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{accountId}\n  method: get\n  operationId: GetPortfolios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:portfolios:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/{portfolioId}/portfolio_fields\n  method: get\n  operationId: GetPortfolioCustomFields\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:portfolios:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/{portfolioId}/terminology\n  method: get\n  operationId: GetPortfolioTerminology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:portfolios:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{accountId}\n  method: get\n  operationId: GetWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:workspace-meta:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: get\n  operationId: GetWorkspacesByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:workspace-meta:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspaceId}/custom_fields\n\
  \  method: get\n  operationId: GetCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:workspace-meta:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspaceId}/terminology\n  method: get\n  operationId: GetTerminology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:workspace-meta:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/api-key\n  method: get\n  operationId: GetMyApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item/{itemId}\n  method: get\n  operationId: GetItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:items:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item/{itemId}\n\
  \  method: delete\n  operationId: DeleteItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - delete:items:craft\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item/{itemId}/flat\n  method: get\n  operationId: GetItemFlat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:items:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspaceId}/items\n  method: get\n  operationId: GetItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:items:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspaceId}/items/flat\n  method: get\n  operationId: GetItemsFlat\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:items:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio_item/{itemId}\n  method: get\n  operationId: GetInitiative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:portfolios:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/{portfolioId}/items\n  method: get\n  operationId: GetInitiatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:portfolios:craft\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item\n  method: post\n  operationId: CreateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:items:craft\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /item\n  method: put\n  operationId: UpdateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:items:craft\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craft-io/refs/heads/main/agentic-access/craft-io-agentic-access.yml
summary_line: 27 operations · 5 acting
tags:
- Product Management
- Roadmaps
- OKRs
- Backlog
- Feedback
- Portfolio
- Specifications
---
