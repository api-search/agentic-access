---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 8
api_specs:
- filename: tektolo-com-catalog-api-openapi.yml
  format: yaml
  label: tektolo-com Catalog API
  slug: tektolo-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-catalog-api-openapi.yml
- filename: tektolo-com-deposit-settlement-api-openapi.yml
  format: yaml
  label: tektolo-com Deposit Settlement API
  slug: tektolo-com-deposit-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-deposit-settlement-api-openapi.yml
- filename: tektolo-com-feedback-api-openapi.yml
  format: yaml
  label: tektolo-com Feedback API
  slug: tektolo-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-feedback-api-openapi.yml
- filename: tektolo-com-keys-api-openapi.yml
  format: yaml
  label: tektolo-com Keys API
  slug: tektolo-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-keys-api-openapi.yml
- filename: tektolo-com-property-turnover-api-openapi.yml
  format: yaml
  label: tektolo-com Property Turnover API
  slug: tektolo-com-property-turnover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-property-turnover-api-openapi.yml
- filename: tektolo-com-rules-history-api-openapi.yml
  format: yaml
  label: tektolo-com rules history API
  slug: tektolo-com-rules-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-rules-history-api-openapi.yml
- filename: tektolo-com-verify-api-openapi.yml
  format: yaml
  label: tektolo-com Verify API
  slug: tektolo-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-verify-api-openapi.yml
- filename: tektolo-com-x402-api-openapi.yml
  format: yaml
  label: tektolo-com X402 API
  slug: tektolo-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tektolo-com/openapi/tektolo-com-x402-api-openapi.yml
consequence_counts:
  physical: 14
  read: 8
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tektolo Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/rules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/settle/render/csv
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/settle/render/html
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/settle/render/pdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/settle/render/tenant_html
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-settlement/settle/render/tenant_pdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/deposit-settlement/settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/deposit-settlement/settle/render/csv
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/deposit-settlement/settle/render/html
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/deposit-settlement/settle/render/pdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/deposit-settlement/settle/render/tenant_html
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/deposit-settlement/settle/render/tenant_pdf
operation_count: 39
overview: 'tektolo-com exposes 39 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 17 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tektolo-com
provider_slug: tektolo-com
slug: tektolo-com-agentic-access
source_filename: tektolo-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/tektolo-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 8\n    acting: 31\n  by_consequence:\n    read: 8\n    physical: 14\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/keys\n  method: post\n  operationId: create_key_v1_keys_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities\n  method: get\n  operationId: list_capabilities_v1_capabilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/capabilities/{capability_id}\n  method: get\n  operationId: get_capability_v1_capabilities__capability_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deposit-settlement/settle\n  method: post\n  operationId: deposit_settlement_settle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deposit-settlement/settle/render/html\n  method: post\n  operationId: deposit_settlement_settle_render_html\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deposit-settlement/settle/render/pdf\n  method: post\n  operationId: deposit_settlement_settle_render_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deposit-settlement/settle/render/csv\n  method: post\n  operationId: deposit_settlement_settle_render_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deposit-settlement/settle/render/tenant_html\n  method: post\n  operationId: deposit_settlement_settle_render_tenant_html\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deposit-settlement/settle/render/tenant_pdf\n  method: post\n  operationId: deposit_settlement_settle_render_tenant_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/deposit-settlement/rules\n  method: post\n  operationId: deposit_settlement_rules\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/quick_estimate\n  method: post\n  operationId: property_turnover_quick_estimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/scope\n  method: post\n  operationId: property_turnover_scope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/scope/render/xlsx\n  method: post\n  operationId: property_turnover_scope_render_xlsx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/scope/render/html\n  method: post\n  operationId: property_turnover_scope_render_html\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/scope/render/csv\n\
  \  method: post\n  operationId: property_turnover_scope_render_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/scope/render/vendor_csv\n  method: post\n  operationId: property_turnover_scope_render_vendor_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/scope/render/bids_html\n  method: post\n  operationId: property_turnover_scope_render_bids_html\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/issue_codes\n  method: post\n  operationId: property_turnover_issue_codes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/issue_codes\n  method: get\n  operationId: property_turnover_issue_codes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/deposit-settlement/settle\n  method: post\n  operationId: x402_deposit_settlement_settle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/deposit-settlement/settle/render/html\n  method: post\n  operationId: x402_deposit_settlement_settle_render_html\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/deposit-settlement/settle/render/pdf\n  method: post\n  operationId: x402_deposit_settlement_settle_render_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/deposit-settlement/settle/render/csv\n  method: post\n  operationId: x402_deposit_settlement_settle_render_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/deposit-settlement/settle/render/tenant_html\n  method: post\n  operationId: x402_deposit_settlement_settle_render_tenant_html\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/deposit-settlement/settle/render/tenant_pdf\n  method: post\n  operationId: x402_deposit_settlement_settle_render_tenant_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/quick_estimate\n  method: post\n  operationId: x402_property_turnover_quick_estimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/scope\n  method:\
  \ post\n  operationId: x402_property_turnover_scope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/scope/render/xlsx\n  method: post\n  operationId: x402_property_turnover_scope_render_xlsx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/scope/render/html\n  method: post\n  operationId: x402_property_turnover_scope_render_html\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/scope/render/csv\n  method: post\n  operationId: x402_property_turnover_scope_render_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/scope/render/vendor_csv\n  method: post\n  operationId: x402_property_turnover_scope_render_vendor_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/property-turnover/scope/render/bids_html\n\
  \  method: post\n  operationId: x402_property_turnover_scope_render_bids_html\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: post\n  operationId: post_feedback_v1_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules/history\n  method: get\n  operationId: rule_history_v1_rules_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/rules/changes\n  method: get\n  operationId: rule_changes_v1_rules_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/cites\n  method: get\n  operationId: rule_cites_v1_rules_cites_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/as-of\n  method: get\n  operationId: rule_as_of_v1_rules_as_of_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify\n  method: post\n  operationId: verify_api_v1_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/property-turnover/read_document\n  method: post\n  operationId: property_turnover_read_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/tektolo-com/agentic-access/tektolo-com-agentic-access.yml
summary_line: 39 operations · 31 acting
tags:
- Company
- Tools
- Artificial Intelligence
- Automation
- Reliability
---
