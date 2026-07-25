---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 15
api_specs:
- filename: story-protocol-collections-api-openapi.yml
  format: yaml
  label: Story Protocol Collections API
  slug: story-protocol-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-collections-api-openapi.yml
- filename: story-protocol-disputes-api-openapi.yml
  format: yaml
  label: Story Protocol Disputes API
  slug: story-protocol-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-disputes-api-openapi.yml
- filename: story-protocol-ipassets-api-openapi.yml
  format: yaml
  label: Story Protocol IPAssets API
  slug: story-protocol-ipassets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-ipassets-api-openapi.yml
- filename: story-protocol-ipgroup-api-openapi.yml
  format: yaml
  label: Story Protocol IPGroup API
  slug: story-protocol-ipgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-ipgroup-api-openapi.yml
- filename: story-protocol-iplicenseterms-api-openapi.yml
  format: yaml
  label: Story Protocol IPLicenseTerms API
  slug: story-protocol-iplicenseterms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-iplicenseterms-api-openapi.yml
- filename: story-protocol-licenses-api-openapi.yml
  format: yaml
  label: Story Protocol Licenses API
  slug: story-protocol-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licenses-api-openapi.yml
- filename: story-protocol-licensetemplates-api-openapi.yml
  format: yaml
  label: Story Protocol LicenseTemplates API
  slug: story-protocol-licensetemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licensetemplates-api-openapi.yml
- filename: story-protocol-licenseterms-api-openapi.yml
  format: yaml
  label: Story Protocol LicenseTerms API
  slug: story-protocol-licenseterms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licenseterms-api-openapi.yml
- filename: story-protocol-licensetokens-api-openapi.yml
  format: yaml
  label: Story Protocol LicenseTokens API
  slug: story-protocol-licensetokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licensetokens-api-openapi.yml
- filename: story-protocol-modules-api-openapi.yml
  format: yaml
  label: Story Protocol Modules API
  slug: story-protocol-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-modules-api-openapi.yml
- filename: story-protocol-permissions-api-openapi.yml
  format: yaml
  label: Story Protocol Permissions API
  slug: story-protocol-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-permissions-api-openapi.yml
- filename: story-protocol-royalties-api-openapi.yml
  format: yaml
  label: Story Protocol Royalties API
  slug: story-protocol-royalties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-royalties-api-openapi.yml
- filename: story-protocol-transactions-api-openapi.yml
  format: yaml
  label: Story Protocol Transactions API
  slug: story-protocol-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-transactions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Story Protocol Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v3/royalties/payments
operation_count: 33
overview: 'Story Protocol exposes 33 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 17 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Story Protocol
provider_slug: story-protocol
slug: story-protocol-agentic-access
source_filename: story-protocol-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/story-protocol-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 18\n    connected: 15\n  by_consequence:\n    write: 17\n    read: 15\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v3/assets\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/assets/edges\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/assets/{assetId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/assets/{assetId}/metadata\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/collections\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/collections/{collectionId}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/detailed-ip-license-terms\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/disputes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/disputes/{disputeId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/ip-group-edges\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/ip-groups\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/licenses/ip/terms\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/licenses/ip/terms/{ipId}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/licenses/mintingfees\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/licenses/mintingfees/{licenseMintingFeePaidId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/licenses/templates\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v3/licenses/templates/{licenseTemplateId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/licenses/terms\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/licenses/terms/default\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/licenses/terms/{licenseTermId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/licenses/tokens\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/licenses/tokens/{licenseTokenId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/modules\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/modules/{moduleId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v3/permissions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/permissions/{permissionId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/royalties/payments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/royalties/payments/{royaltyPayId}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/transactions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/transactions/latest\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/transactions/{trxId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/licenses/mintingfees\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/licenses/mintingfees/{licenseMintingFeePaidId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/agentic-access/story-protocol-agentic-access.yml
summary_line: 33 operations · 18 acting
tags:
- Company
- Blockchain
- Intellectual Property
- Licensing
- Royalties
- Web3
- NFT
- API
- Developer Tools
---
