---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: crawlgraph-v1-api-openapi.yml
  format: yaml
  label: CrawlGraph V1 API
  slug: crawlgraph-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlgraph/refs/heads/main/openapi/crawlgraph-v1-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crawlgraph Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'CrawlGraph exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CrawlGraph
provider_slug: crawlgraph
slug: crawlgraph-agentic-access
source_filename: crawlgraph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: generated\nsource: openapi/crawlgraph-v1-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/backlinks\n  method: post\n  operationId: v1_lookup_backlinks_api_v1_backlinks_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: metered\n  correction:\n    from: {action-class: acting, consequence: write}\n    reason: >-\n      The HTTP-method heuristic read POST as a write. It is not: this is a read-only backlink\n      lookup that\
  \ uses POST only to carry a JSON request body. The provider says so on two\n      surfaces — the MCP tool that wraps this operation publishes\n      annotations {readOnlyHint: true, destructiveHint: false, idempotentHint: true}\n      (probed at https://crawlgraph.com/mcp), and the docs describe it as a \"synchronous backlink\n      lookup\". It has no persistent side effect other than decrementing the caller's monthly\n      quota, which is why audit is `metered` rather than `none`.\n    method: searched\n    source: https://crawlgraph.com/docs/api\n- path: /api/v1/free-key\n  method: post\n  operationId: request_free_key_api_v1_free_key_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/releases\n  method: get\n  operationId: v1_list_releases_api_v1_releases_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gap-analysis\n  method: post\n  operationId: v1_gap_submit_api_v1_gap_analysis_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n  note: >-\n    Kept as a write. The analysis itself is read-only, but the call creates a durable, owner-scoped\n    job resource retained for 7 days AND spends one of 50 monthly gap jobs. The docs state failed\n    jobs do not refund quota in v1, so a retry is not free and there is no cancel operation —\n    see the reversibility block in conventions/crawlgraph-conventions.yml.\n- path: /api/v1/gap-analysis/{job_id}\n  method: get\n  operationId: v1_gap_poll_api_v1_gap_analysis__job_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/changes\n  method: get\n  operationId: v1_changes_api_v1_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlgraph/refs/heads/main/agentic-access/crawlgraph-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- SEO
- backlink-intelligence
- MarTech
- Competitive Intelligence
- Web Data
- Common-Crawl
- link-building
- Developer Tools
- MCP
---
