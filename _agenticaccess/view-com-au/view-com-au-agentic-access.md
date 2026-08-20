---
acting_count: 0
action_class_counts:
  acting: 0
  connected: 3
consequence_counts:
  physical: 0
  read: 3
  safety-critical: 0
  write: 0
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: View Com Au Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'View.com.au exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: View.com.au
provider_slug: view-com-au
slug: view-com-au-agentic-access
source_filename: view-com-au-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: mcp/view-com-au-mcp-tools.json\nnotes: >-\n  A recommended x-agentic-access execution contract per MCP tool, following the\n  Curity \"Access Intelligence\" model. This is a governance starting point\n  authored by API Evangelist, not a claim published by View.com.au — the\n  provider publishes no agent access guidance at all. There is no OpenAPI, so\n  the unit of access here is the MCP tool rather than an operationId. `audience`\n  is left null to be bound per deployment.\n\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n    acting: 0\n  by_consequence:\n    read: 3\n    write: 0\n    physical: 0\n    safety-critical: 0\n  human_in_the_loop: 0\n  audit_required: 0\n  note: >-\n    The published surface is entirely read-only, which is why every contract\n    below sits in the lowest consequence band. The real agentic risk here is not\n    mutation, it is unattributable bulk read: there is no credential,\
  \ so there\n    is no identity, no attribution and no quota negotiation — only an anonymous\n    100-request/300-second ceiling shared by every caller from the same origin.\n\noperations:\n- operation: propertySearch\n  surface: mcp\n  transport: https://mcp.view.com.au/mcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: null\n    scope: property:search\n    token:\n      required: false\n      ttl-max: 3600\n      note: No credential exists. Rate limiting is the only control.\n    escalation: none\n    human-in-the-loop: not-required\n    audit: recommended\n    data-sensitivity: >-\n      Returns identified third-party records — property addresses, geocodes,\n      prices, agency and agent names, emails and phone numbers. Personal data\n      under the Australian Privacy Act, and proprietary portal content that is\n      free to call but not open-licensed.\n    rate-guidance: >-\n      100 requests per 300 seconds, shared and anonymous. Paginate\
  \ deliberately;\n      an agent cannot request more quota because it cannot identify itself.\n- operation: propertyDetail\n  surface: mcp\n  transport: https://mcp.view.com.au/mcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: null\n    scope: property:read\n    token:\n      required: false\n      ttl-max: 3600\n    escalation: none\n    human-in-the-loop: not-required\n    audit: recommended\n    data-sensitivity: >-\n      Higher than search: returns agent email, phone and mobile, inspection\n      schedules, floor plans and the Statement of Information. Do not\n      redistribute agent contact details or use them for outbound contact.\n- operation: offMarketPropertyDetail\n  surface: mcp\n  transport: https://mcp.view.com.au/mcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: null\n    scope: property:offmarket:read\n    token:\n      required: false\n      ttl-max: 3600\n    escalation: none\n    human-in-the-loop:\
  \ not-required\n    audit: required\n    data-sensitivity: >-\n      The most sensitive of the three. Off-market records describe properties\n      that are NOT listed for sale — an owner has not chosen to publish them —\n      and include automated price estimates, property history, zoning and\n      planning overlays. Treat estimates as View's opinion, never as a\n      valuation, and never present them to a consumer as an appraisal.\n    escalation-note: >-\n      Off-market lookups are the operation most likely to be repurposed for\n      unsolicited vendor prospecting. Bind an audience and require an audit\n      trail before allowing an agent to run these at volume.\n\ndeployment_guidance:\n- Cache aggressively; the quota is the binding constraint and there is no way to raise it.\n- Attribute nothing to a user identity — the surface returns no identity and accepts none.\n- Re-read tools/list each session; the server advertises listChanged and publishes no versioning or deprecation\
  \ policy.\n- Treat the absence of terms governing the MCP surface as unresolved rather than as permission; the site's Terms of Use govern the website, and no separate API or agent terms were found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/view-com-au/refs/heads/main/agentic-access/view-com-au-agentic-access.yml
summary_line: 3 operations
tags:
- Real-Estate
- Australia
- Property Listings
- Property Portal
- PropTech
- Rentals
- Off-Market Property Data
- MCP
- agent-native
---
