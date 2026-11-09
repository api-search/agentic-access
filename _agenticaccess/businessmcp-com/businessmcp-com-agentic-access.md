---
acting_count: 69
action_class_counts:
  acting: 69
  connected: 34
api_specs:
- filename: businessmcp-com-account-api-openapi.yml
  format: yaml
  label: BusinessMCP Account API
  slug: businessmcp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-account-api-openapi.yml
- filename: businessmcp-com-assistant-api-openapi.yml
  format: yaml
  label: BusinessMCP Assistant API
  slug: businessmcp-com-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-assistant-api-openapi.yml
- filename: businessmcp-com-companies-api-openapi.yml
  format: yaml
  label: BusinessMCP Companies API
  slug: businessmcp-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-companies-api-openapi.yml
- filename: businessmcp-com-email-api-openapi.yml
  format: yaml
  label: BusinessMCP Email API
  slug: businessmcp-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-email-api-openapi.yml
- filename: businessmcp-com-events-api-api-openapi.yml
  format: yaml
  label: BusinessMCP Events API
  slug: businessmcp-com-events-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-events-api-api-openapi.yml
- filename: businessmcp-com-export-api-openapi.yml
  format: yaml
  label: BusinessMCP Export API
  slug: businessmcp-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-export-api-openapi.yml
- filename: businessmcp-com-free-api-openapi.yml
  format: yaml
  label: BusinessMCP Free API
  slug: businessmcp-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-free-api-openapi.yml
- filename: businessmcp-com-ip-api-openapi.yml
  format: yaml
  label: BusinessMCP Ip API
  slug: businessmcp-com-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-ip-api-openapi.yml
- filename: businessmcp-com-meta-api-openapi.yml
  format: yaml
  label: BusinessMCP Meta API
  slug: businessmcp-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-meta-api-openapi.yml
- filename: businessmcp-com-people-api-openapi.yml
  format: yaml
  label: BusinessMCP People API
  slug: businessmcp-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-people-api-openapi.yml
- filename: businessmcp-com-read-api-api-openapi.yml
  format: yaml
  label: BusinessMCP Read API
  slug: businessmcp-com-read-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-read-api-api-openapi.yml
- filename: businessmcp-com-signup-api-openapi.yml
  format: yaml
  label: BusinessMCP Signup API
  slug: businessmcp-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-signup-api-openapi.yml
- filename: businessmcp-com-sites-api-openapi.yml
  format: yaml
  label: BusinessMCP Sites API
  slug: businessmcp-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-sites-api-openapi.yml
- filename: businessmcp-com-technology-api-openapi.yml
  format: yaml
  label: BusinessMCP Technology API
  slug: businessmcp-com-technology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-technology-api-openapi.yml
- filename: businessmcp-com-tools-api-openapi.yml
  format: yaml
  label: BusinessMCP Tools API
  slug: businessmcp-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-tools-api-openapi.yml
- filename: businessmcp-com-traffic-api-openapi.yml
  format: yaml
  label: BusinessMCP Traffic API
  slug: businessmcp-com-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-traffic-api-openapi.yml
- filename: businessmcp-com-trust-api-openapi.yml
  format: yaml
  label: BusinessMCP Trust API
  slug: businessmcp-com-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-trust-api-openapi.yml
- filename: businessmcp-com-usage-api-openapi.yml
  format: yaml
  label: BusinessMCP Usage API
  slug: businessmcp-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-usage-api-openapi.yml
- filename: businessmcp-com-visibility-api-openapi.yml
  format: yaml
  label: BusinessMCP Visibility API
  slug: businessmcp-com-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-visibility-api-openapi.yml
consequence_counts:
  physical: 2
  read: 34
  safety-critical: 2
  write: 65
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Businessmcp Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /skills/scan
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tools/fp.skill.scan/call
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/topup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /track
operation_count: 103
overview: 'BusinessMCP exposes 103 API operations that an AI agent could call, of which 69 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 65 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BusinessMCP
provider_slug: businessmcp-com
slug: businessmcp-com-agentic-access
source_filename: businessmcp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/businessmcp-com-hub-openapi.json, openapi/businessmcp-com-v1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 103\n  by_action_class:\n    acting: 69\n    connected: 34\n  by_consequence:\n    write: 65\n    read: 34\n    safety-critical: 2\n    physical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /tools/fp.company.lookup/call\n  method: post\n  operationId: call_fp_company_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /companies/{domain}\n  method: get\n  operationId: fp_company_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.company.linkedin/call\n  method: post\n  operationId: call_fp_company_linkedin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{domain}/linkedin\n  method: get\n  operationId: fp_company_linkedin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.company.bulk/call\n  method: post\n  operationId: call_fp_company_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/bulk\n  method: post\n  operationId: fp_company_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.company.liveness/call\n  method: post\n  operationId: call_fp_company_liveness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{domain}/status\n  method: get\n  operationId: fp_company_liveness\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.company.email_pattern/call\n  method: post\n  operationId: call_fp_company_email_pattern\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{domain}/email-pattern\n  method: get\n  operationId: fp_company_email_pattern\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.company.contacts/call\n  method: post\n  operationId: call_fp_company_contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{domain}/contacts\n  method: get\n  operationId: fp_company_contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.company.logo/call\n  method: post\n  operationId: call_fp_company_logo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{domain}/logo\n  method: get\n  operationId: fp_company_logo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.company.search/call\n\
  \  method: post\n  operationId: call_fp_company_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/search\n  method: post\n  operationId: fp_company_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.ip.lookup/call\n  method: post\n  operationId: call_fp_ip_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ip/{ip}\n  method: get\n  operationId: fp_ip_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.ip.bulk/call\n  method: post\n  operationId: call_fp_ip_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip/bulk\n  method: post\n  operationId: fp_ip_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.ip.geo/call\n  method: post\n  operationId:\
  \ call_fp_ip_geo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/{ip}\n  method: get\n  operationId: fp_ip_geo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.ip.geo_bulk/call\n  method: post\n  operationId: call_fp_ip_geo_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/bulk\n  method: post\n  operationId: fp_ip_geo_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.tech.lookup/call\n  method: post\n  operationId: call_fp_tech_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tech/{domain}\n  method: get\n  operationId: fp_tech_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.tech.search/call\n  method: post\n  operationId: call_fp_tech_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tech/search\n  method: post\n  operationId: fp_tech_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.traffic.estimate/call\n  method: post\n  operationId: call_fp_traffic_estimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /traffic/{domain}\n  method: get\n  operationId: fp_traffic_estimate\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.traffic.rank/call\n  method: post\n  operationId: call_fp_traffic_rank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rank/{domain}\n  method: get\n  operationId: fp_traffic_rank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.network.classify/call\n  method: post\n  operationId: call_fp_network_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /network/classify\n  method: post\n  operationId: fp_network_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.site.ai_readiness/call\n  method: post\n  operationId: call_fp_site_ai_readiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{domain}/ai-readiness\n  method: get\n  operationId: fp_site_ai_readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /tools/fp.site.ai_crawlers/call\n  method: post\n  operationId: call_fp_site_ai_crawlers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{domain}/ai-crawlers\n  method: get\n  operationId: fp_site_ai_crawlers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.site.webmcp/call\n  method: post\n  operationId: call_fp_site_webmcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sites/{domain}/webmcp\n  method: get\n  operationId: fp_site_webmcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.site.email_auth/call\n  method: post\n  operationId: call_fp_site_email_auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{domain}/email-auth\n  method: get\n  operationId: fp_site_email_auth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.mcp.probe/call\n  method: post\n  operationId: call_fp_mcp_probe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/scan\n  method: post\n  operationId: fp_mcp_probe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.lead.check/call\n  method: post\n  operationId: call_fp_lead_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/check\n  method: post\n  operationId: fp_lead_check\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.email.verify/call\n  method: post\n  operationId: call_fp_email_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/verify\n  method: post\n  operationId: fp_email_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.email.verify_bulk/call\n  method: post\n\
  \  operationId: call_fp_email_verify_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/verify/bulk\n  method: post\n  operationId: fp_email_verify_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.traffic.classify/call\n  method: post\n  operationId: call_fp_traffic_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /traffic/classify\n  method: post\n  operationId: fp_traffic_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.skill.scan/call\n  method: post\n  operationId: call_fp_skill_scan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /skills/scan\n  method: post\n  operationId: fp_skill_scan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tools/fp.ai.visibility_probe/call\n  method: post\n  operationId: call_fp_ai_visibility_probe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-visibility/probe\n  method: post\n  operationId: fp_ai_visibility_probe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.mcp.monitor.create/call\n  method: post\n  operationId:\
  \ call_fp_mcp_monitor_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/monitors\n  method: post\n  operationId: fp_mcp_monitor_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/monitors\n  method: get\n  operationId: fp_mcp_monitor_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.mcp.monitor.list/call\n  method: post\n  operationId: call_fp_mcp_monitor_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.mcp.monitor.events/call\n  method: post\n  operationId: call_fp_mcp_monitor_events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/monitors/events\n  method: get\n  operationId: fp_mcp_monitor_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/fp.mcp.monitor.update/call\n  method: post\n  operationId: call_fp_mcp_monitor_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/monitors/{monitor_id}\n  method: post\n  operationId: fp_mcp_monitor_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.mcp.monitor.delete/call\n  method: post\n  operationId: call_fp_mcp_monitor_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/monitors/{monitor_id}/delete\n  method: post\n  operationId: fp_mcp_monitor_delete\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.people.search/call\n  method: post\n  operationId: call_fp_people_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/search\n  method: post\n  operationId: fp_people_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.people.email_finder/call\n  method:\
  \ post\n  operationId: call_fp_people_email_finder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/email-finder\n  method: post\n  operationId: fp_people_email_finder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.people.enrich/call\n  method: post\n  operationId: call_fp_people_enrich\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /people/enrich\n  method: post\n  operationId: fp_people_enrich\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.people.linkedin_to_email/call\n  method: post\n  operationId: call_fp_people_linkedin_to_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/linkedin-to-email\n  method: post\n  operationId: fp_people_linkedin_to_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/fp.people.email_to_linkedin/call\n  method: post\n  operationId: call_fp_people_email_to_linkedin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/email-to-linkedin\n  method: post\n  operationId: fp_people_email_to_linkedin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools\n  method: get\n  operationId: list_tools\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup/challenge\n  method: get\n  operationId: signup_challenge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup\n  method: post\n  operationId: signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signup/verify\n  method: post\n  operationId: signup_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /billing\n  method: get\n  operationId: billing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/topup\n  method: post\n  operationId: billing_topup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/auto-topup\n  method: post\n  operationId: billing_auto_topup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /free/ip\n\
  \  method: get\n  operationId: free_ip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/email\n  method: get\n  operationId: free_email\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/company\n  method: get\n  operationId: free_company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export\n  method: get\n  operationId: exportCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /track\n  method: post\n  operationId: trackEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identify\n  method: post\n  operationId: identify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group\n  method: post\n  operationId: group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs\n  method: post\n  operationId: startRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs\n  method: get\n  operationId:\
  \ getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup/start\n  method: post\n  operationId: signupStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signup/verify\n  method: post\n  operationId: signupVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/businessmcp-com/agentic-access/businessmcp-com-agentic-access.yml
summary_line: 103 operations · 69 acting · 2 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Marketing
- Sales
- Automation
- Platform
---
