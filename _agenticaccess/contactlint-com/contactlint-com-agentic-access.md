---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 30
api_specs:
- filename: contactlint-com-openapi.json
  format: json
  label: ContactLint API
  slug: contactlint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-openapi.json
- filename: contactlint-com-demo-api-openapi.yml
  format: yaml
  label: contactlint-com Demo API
  slug: contactlint-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-demo-api-openapi.yml
- filename: contactlint-com-demo-preview-api-openapi.yml
  format: yaml
  label: contactlint-com Demo Preview API
  slug: contactlint-com-demo-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-demo-preview-api-openapi.yml
- filename: contactlint-com-demo-preview-rotation-api-openapi.yml
  format: yaml
  label: contactlint-com Demo Preview Rotation API
  slug: contactlint-com-demo-preview-rotation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-demo-preview-rotation-api-openapi.yml
- filename: contactlint-com-domain-api-openapi.yml
  format: yaml
  label: contactlint-com Domain API
  slug: contactlint-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-domain-api-openapi.yml
- filename: contactlint-com-go-api-openapi.yml
  format: yaml
  label: contactlint-com Go API
  slug: contactlint-com-go-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-go-api-openapi.yml
- filename: contactlint-com-health-api-openapi.yml
  format: yaml
  label: contactlint-com Health API
  slug: contactlint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-health-api-openapi.yml
- filename: contactlint-com-lookup-api-openapi.yml
  format: yaml
  label: contactlint-com Lookup API
  slug: contactlint-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-lookup-api-openapi.yml
- filename: contactlint-com-metrics-api-openapi.yml
  format: yaml
  label: contactlint-com Metrics API
  slug: contactlint-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-metrics-api-openapi.yml
- filename: contactlint-com-monitor-api-openapi.yml
  format: yaml
  label: contactlint-com Monitor API
  slug: contactlint-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-monitor-api-openapi.yml
- filename: contactlint-com-payment-change-check-api-openapi.yml
  format: yaml
  label: contactlint-com Payment Change Check API
  slug: contactlint-com-payment-change-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-payment-change-check-api-openapi.yml
- filename: contactlint-com-report-api-openapi.yml
  format: yaml
  label: contactlint-com Report API
  slug: contactlint-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-report-api-openapi.yml
- filename: contactlint-com-reports-api-openapi.yml
  format: yaml
  label: contactlint-com Reports API
  slug: contactlint-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-reports-api-openapi.yml
- filename: contactlint-com-robots-txt-api-openapi.yml
  format: yaml
  label: contactlint-com Robots.txt API
  slug: contactlint-com-robots-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-robots-txt-api-openapi.yml
- filename: contactlint-com-sitemap-xml-api-openapi.yml
  format: yaml
  label: contactlint-com Sitemap.xml API
  slug: contactlint-com-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-sitemap-xml-api-openapi.yml
consequence_counts:
  physical: 2
  read: 30
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Contactlint Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-change-check/api
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-change-check/waitlist
operation_count: 34
overview: 'contactlint-com exposes 34 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: contactlint-com
provider_slug: contactlint-com
slug: contactlint-com-agentic-access
source_filename: contactlint-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/contactlint-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 4\n    connected: 30\n  by_consequence:\n    write: 2\n    read: 30\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /monitor\n  method: post\n  operationId: monitor_signup_monitor_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitor/confirm\n  method: get\n  operationId: monitor_confirm_monitor_confirm_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor/unsubscribe\n  method: get\n  operationId: monitor_unsubscribe_monitor_unsubscribe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor/manage\n  method: get\n  operationId: monitor_manage_monitor_manage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor/manage\n  method: post\n  operationId: monitor_manage_save_monitor_manage_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /payment-change-check\n  method: get\n  operationId: paycheck_page_payment_change_check_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-change-check\n  method: head\n  operationId: paycheck_page_payment_change_check_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-change-check/api\n  method: post\n  operationId: paycheck_api_payment_change_check_api_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-change-check/sample/{name}\n  method: get\n\
  \  operationId: paycheck_sample_payment_change_check_sample__name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-change-check/waitlist\n  method: post\n  operationId: paycheck_waitlist_payment_change_check_waitlist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-change-check/confirm\n  method: get\n  operationId: paycheck_confirm_payment_change_check_confirm_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-change-check/unsubscribe\n  method: get\n\
  \  operationId: paycheck_unsubscribe_payment_change_check_unsubscribe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: metrics_metrics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{domain}\n  method: get\n  operationId: lookup_lookup__domain__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain/{domain}/dns\n  method: get\n  operationId: dns_only_domain__domain__dns_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain/{domain}/ssl\n  method: get\n  operationId: ssl_only_domain__domain__ssl_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain/{domain}/whois\n  method: get\n  operationId: whois_only_domain__domain__whois_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain/{domain}/subdomains\n  method: get\n  operationId: subs_only_domain__domain__subdomains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain/{domain}/email-security\n  method: get\n  operationId: email_only_domain__domain__email_security_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demo/{domain}\n  method: get\n  operationId: demo_lookup_demo__domain__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demo-preview/{domain}\n  method: get\n  operationId: demo_preview_demo_preview__domain__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demo-preview-rotation\n  method: get\n  operationId: demo_preview_rotation_demo_preview_rotation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: get\n  operationId: reports_index_reports_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: head\n  operationId: reports_index_reports_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{domain}\n  method: head\n  operationId: report_report__domain__head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{domain}\n  method: get\n  operationId: report_report__domain__head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{domain}/subdomains-status\n  method: get\n  operationId: report_subdomains_status_report__domain__subdomains_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: sitemap_sitemap_xml_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: head\n  operationId: sitemap_sitemap_xml_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /go/rapidapi\n  method: get\n  operationId: go_rapidapi_go_rapidapi_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /go/rapidapi\n  method: head\n  operationId: go_rapidapi_go_rapidapi_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  operationId: robots_robots_txt_head\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: head\n  operationId: robots_robots_txt_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/contactlint-com/agentic-access/contactlint-com-agentic-access.yml
summary_line: 34 operations · 4 acting
tags:
- Email Verification
- Phone Validation
- MCP
- Developer Tools
- Company
---
