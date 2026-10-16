---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 56
api_specs:
- filename: adslighthouse-account-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Account API
  slug: adslighthouse-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-account-api-openapi.yml
- filename: adslighthouse-alerts-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Alerts API
  slug: adslighthouse-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-alerts-api-openapi.yml
- filename: adslighthouse-checks-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Checks API
  slug: adslighthouse-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-checks-api-openapi.yml
- filename: adslighthouse-google-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Google API
  slug: adslighthouse-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-google-api-openapi.yml
- filename: adslighthouse-keywords-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Keywords API
  slug: adslighthouse-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-keywords-api-openapi.yml
- filename: adslighthouse-matching-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Matching API
  slug: adslighthouse-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-matching-api-openapi.yml
- filename: adslighthouse-observations-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Observations API
  slug: adslighthouse-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-observations-api-openapi.yml
- filename: adslighthouse-policy-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Policy API
  slug: adslighthouse-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-policy-api-openapi.yml
- filename: adslighthouse-prices-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Prices API
  slug: adslighthouse-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-prices-api-openapi.yml
- filename: adslighthouse-projects-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Projects API
  slug: adslighthouse-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-projects-api-openapi.yml
- filename: adslighthouse-redirect-chains-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Redirect chains API
  slug: adslighthouse-redirect-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-redirect-chains-api-openapi.yml
- filename: adslighthouse-reports-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Reports API
  slug: adslighthouse-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-reports-api-openapi.yml
- filename: adslighthouse-router-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Router API
  slug: adslighthouse-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-router-api-openapi.yml
- filename: adslighthouse-team-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Team API
  slug: adslighthouse-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-team-api-openapi.yml
consequence_counts:
  physical: 2
  read: 56
  safety-critical: 4
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Adslighthouse Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /alert-rules/{rule_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /projects/{project_id}/keywords
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /projects/{project_id}/keywords/{keyword_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /team/invitations/{invitation_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /alert-rules/{rule_id}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /team/invitations/{invitation_id}/resend
operation_count: 88
overview: 'Ads Lighthouse exposes 88 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 56 read, 26 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ads Lighthouse
provider_slug: adslighthouse
slug: adslighthouse-agentic-access
source_filename: adslighthouse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/adslighthouse-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 88\n  by_action_class:\n    connected: 56\n    acting: 32\n  by_consequence:\n    read: 56\n    write: 26\n    safety-critical: 4\n    physical: 2\n  human_in_the_loop_required: 4\noperations:\n- path: /account\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: list_projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /projects\n  method: post\n  operationId: create_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: get\n  operationId: get_project_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: patch\n  operationId: update_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: delete_project\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/keywords\n  method: get\n  operationId: list_keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/keywords\n  method: post\n  operationId: add_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/keywords\n  method: delete\n  operationId: remove_keywords\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /projects/{project_id}/keywords/{keyword_id}\n  method: delete\n  operationId: remove_keyword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /projects/{project_id}/observations\n  method: get\n  operationId: list_observations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/advertisers\n  method: get\n  operationId:\
  \ list_advertisers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/affiliate-findings\n  method: get\n  operationId: list_affiliate_findings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-events\n  method: get\n  operationId: list_alert_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/checks\n  method: post\n  operationId: run_realtime_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /projects/{project_id}/checks\n  method: get\n  operationId: list_check_activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/checks/{run_id}\n  method: get\n  operationId: get_check_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/analytics\n  method: get\n  operationId: get_analytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/organic-observations\n  method: get\n  operationId: list_organic_observations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/summary\n\
  \  method: get\n  operationId: get_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/timeseries\n  method: get\n  operationId: get_timeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/advertisers/{domain}\n  method: get\n  operationId: get_advertiser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/competitors\n  method: get\n  operationId: list_competitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/advertisers/{domain}/classification\n  method: post\n  operationId:\
  \ set_advertiser_classification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/keywords/{keyword_id}/report\n  method: get\n  operationId: get_keyword_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/keywords/{keyword_id}/ads\n  method: get\n  operationId: list_keyword_ads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/affiliate-ids\n  method: get\n  operationId: list_affiliate_ids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/affiliate-findings/{affiliate_id}/status\n  method: post\n  operationId: set_affiliate_case_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/shopping-products\n  method: get\n  operationId: list_shopping_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/exports/paid-results\n  method: get\n  operationId: export_paid_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/exports/paid-results-by-keyword\n\
  \  method: get\n  operationId: export_paid_results_by_keyword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/exports/affiliate-cases\n  method: get\n  operationId: export_affiliate_cases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/advertisers/{domain}/history\n  method: get\n  operationId: get_advertiser_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/advertisers/{domain}/heatmap\n  method: get\n  operationId: get_advertiser_heatmap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/advertisers/{domain}/ad-copy\n\
  \  method: get\n  operationId: list_ad_copy_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/ad-copy-changes\n  method: get\n  operationId: list_ad_copy_changes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-demand\n  method: post\n  operationId: preview_check_demand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitoring-options\n  method: get\n  operationId: get_monitoring_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: search_locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/time-zone\n  method: get\n  operationId: get_time_zone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/time-zone\n  method: patch\n  operationId: update_time_zone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/theme\n  method: get\n  operationId: get_theme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /account/theme\n  method: patch\n  operationId: update_theme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-rules\n  method: get\n  operationId: list_alert_rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-rules\n  method: post\n  operationId: create_alert_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-rules/{rule_id}\n  method: get\n  operationId: get_alert_rule\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-rules/{rule_id}\n  method: post\n  operationId: update_alert_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /alert-rules/{rule_id}\n  method: delete\n  operationId: delete_alert_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-rules/{rule_id}/test\n  method: post\n  operationId: send_test_alert\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-rules/{rule_id}/rotate-secret\n  method: post\n  operationId: rotate_webhook_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-events/{event_id}\n  method: get\n  operationId: get_alert_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team\n  method: get\n  operationId: list_team\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/invitations\n  method: post\n  operationId: invite_team_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/invitations/{invitation_id}/resend\n  method: post\n  operationId: resend_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/invitations/{invitation_id}\n  method: delete\n  operationId: cancel_invitation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /team/members/{user_id}\n  method: post\n  operationId: change_member_role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/members/{user_id}\n  method: delete\n  operationId: remove_team_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /accounts\n  method: get\n  operationId: list_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/overview\n  method: get\n  operationId: get_account_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/email-preferences\n  method: get\n  operationId: get_email_preferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/email-preferences\n  method: post\n  operationId: update_email_preferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /projects/{project_id}/google-connections\n  method: get\n  operationId: list_google_connections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/google-connections/{connection_id}/accounts\n  method: get\n  operationId: list_google_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/google-connections/{connection_id}/ads-report\n  method: get\n  operationId: run_google_ads_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/google-connections/{connection_id}/search-console-report\n  method: get\n  operationId: run_search_console_report\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/redirect-traces\n  method: post\n  operationId: trace_redirects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/redirect-traces\n  method: get\n  operationId: list_redirect_chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/redirect-traces/{trace_id}\n  method: get\n  operationId: get_redirect_chain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /projects/{project_id}/policy-rules\n  method: get\n  operationId: list_policy_rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/policy-rules\n  method: post\n  operationId: create_policy_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/policy-rules/{rule_id}\n  method: get\n  operationId: get_policy_rule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/policy-rules/{rule_id}\n  method: post\n  operationId: update_policy_rule\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/policy-rules/{rule_id}\n  method: delete\n  operationId: delete_policy_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/policy-rule-preview\n  method: post\n  operationId: preview_policy_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /projects/{project_id}/policy-rule-evaluation\n  method: post\n  operationId: evaluate_policy_rules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/policy-cases\n  method: get\n  operationId: list_policy_cases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/policy-cases/{case_id}\n  method: get\n  operationId: get_policy_case\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/policy-cases/{case_id}\n  method: post\n  operationId: update_policy_case\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/policy-cases/{case_id}/evidence\n  method: get\n  operationId: list_policy_case_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/policy-cases/{case_id}/notes\n  method: post\n  operationId: add_policy_case_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/reports\n  method: post\n  operationId: create_report\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/reports\n  method: get\n  operationId: list_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/reports/{report_id}\n  method: get\n  operationId: get_report_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/reports/{report_id}/download-link\n  method: get\n  operationId: get_report_download_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /projects/{project_id}/reports/{report_id}/pdf\n  method: get\n  operationId: download_report_pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/screenshots/{screenshot_id}\n  method: get\n  operationId: download_screenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/shopping-products/{product_id}/image\n  method: get\n  operationId: download_shopping_image\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/landing-screenshots/{page_id}\n  method: get\n  operationId: download_landing_screenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/agentic-access/adslighthouse-agentic-access.yml
summary_line: 88 operations · 32 acting · 4 human-in-the-loop
tags:
- Company
- Advertising
- Monitoring
- BrandProtection
- API
---
