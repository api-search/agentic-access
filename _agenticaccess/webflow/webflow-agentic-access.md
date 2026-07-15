---
acting_count: 116
action_class_counts:
  acting: 116
  connected: 96
api_specs:
- filename: webflow-data-api-openapi.yml
  format: yaml
  label: Webflow Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-data-api-openapi.yml
- filename: webflow-meta-openapi.yml
  format: yaml
  label: Webflow Meta API
  slug: meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-meta-openapi.yml
- filename: webflow-sites-openapi.yml
  format: yaml
  label: Webflow Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-sites-openapi.yml
- filename: webflow-pages-openapi.yml
  format: yaml
  label: Webflow Pages API
  slug: pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-pages-openapi.yml
- filename: webflow-collections-openapi.yml
  format: yaml
  label: Webflow Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-collections-openapi.yml
- filename: webflow-items-openapi.yml
  format: yaml
  label: Webflow CMS Items API
  slug: items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-items-openapi.yml
- filename: webflow-components-openapi.yml
  format: yaml
  label: Webflow Components API
  slug: components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-components-openapi.yml
- filename: webflow-assets-openapi.yml
  format: yaml
  label: Webflow Assets API
  slug: assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-assets-openapi.yml
- filename: webflow-forms-openapi.yml
  format: yaml
  label: Webflow Forms API
  slug: forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-forms-openapi.yml
- filename: webflow-products-openapi.yml
  format: yaml
  label: Webflow Products and SKUs API
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-products-openapi.yml
- filename: webflow-orders-openapi.yml
  format: yaml
  label: Webflow Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-orders-openapi.yml
- filename: webflow-inventory-openapi.yml
  format: yaml
  label: Webflow Inventory API
  slug: inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-inventory-openapi.yml
- filename: webflow-ecommerce-settings-openapi.yml
  format: yaml
  label: Webflow Ecommerce Settings API
  slug: ecommerce-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-ecommerce-settings-openapi.yml
- filename: webflow-webhooks-openapi.yml
  format: yaml
  label: Webflow Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-webhooks-openapi.yml
- filename: webflow-custom-code-openapi.yml
  format: yaml
  label: Webflow Custom Code API
  slug: custom-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-custom-code-openapi.yml
- filename: webflow-comments-openapi.yml
  format: yaml
  label: Webflow Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-comments-openapi.yml
consequence_counts:
  physical: 8
  read: 96
  write: 108
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Webflow Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /sites/{site_id}/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /sites/{site_id}/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site_id}/orders/{order_id}/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site_id}/orders/{order_id}/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site_id}/orders/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site_id}/orders/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site_id}/orders/{order_id}/unfulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site_id}/orders/{order_id}/unfulfill
operation_count: 212
overview: 'Webflow exposes 212 API operations that an AI agent could call, of which 116 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 96 read, 108 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Webflow
provider_slug: webflow
slug: webflow-agentic-access
source_filename: webflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/webflow-assets-openapi.yml, openapi/webflow-collections-openapi.yml, openapi/webflow-comments-openapi.yml,\n  openapi/webflow-components-openapi.yml, openapi/webflow-custom-code-openapi.yml, openapi/webflow-data-api-openapi.yml,\n  openapi/webflow-ecommerce-settings-openapi.yml, openapi/webflow-forms-openapi.yml, openapi/webflow-inventory-openapi.yml,\n  openapi/webflow-items-openapi.yml, openapi/webflow-meta-openapi.yml, openapi/webflow-orders-openapi.yml,\n  openapi/webflow-pages-openapi.yml, openapi/webflow-products-openapi.yml, openapi/webflow-sites-openapi.yml,\n  openapi/webflow-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 212\n  by_action_class:\n    connected:\
  \ 96\n    acting: 116\n  by_consequence:\n    read: 96\n    write: 108\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /sites/{site_id}/assets\n  method: get\n  operationId: list-assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/assets\n  method: post\n  operationId: create-asset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{asset_id}\n  method: get\n  operationId: get-asset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /assets/{asset_id}\n  method: patch\n  operationId: patch-asset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{asset_id}\n  method: delete\n  operationId: delete-asset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/asset_folders\n  method: get\n  operationId: list-asset-folders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/asset_folders\n  method: post\n  operationId: create-asset-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - assets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset_folders/{asset_folder_id}\n  method: get\n  operationId: get-asset-folder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - assets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/collections\n  method: get\n  operationId: list-collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/collections\n\
  \  method: post\n  operationId: create-collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}\n  method: get\n  operationId: collection-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}\n  method: delete\n  operationId: delete-collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /collections/{collection_id}/fields\n  method: post\n  operationId: create-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/fields/{field_id}\n  method: patch\n  operationId: update-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/fields/{field_id}\n  method: delete\n  operationId: delete-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/comments\n  method: get\n  operationId: list-comment-threads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - comments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/comments/{comment_thread_id}\n  method: get\n  operationId: get-comment-thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - comments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/comments/{comment_thread_id}/replies\n  method: get\n  operationId: list-comment-replies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n  \
  \  - comments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components\n  method: get\n  operationId: list-components\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - components:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components/{component_id}/dom\n  method: get\n  operationId: get-component-content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - components:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components/{component_id}/dom\n  method: post\n  operationId: update-component-content\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - components:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/components/{component_id}/properties\n  method: get\n  operationId: get-component-properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - components:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components/{component_id}/properties\n  method: post\n  operationId: update-component-properties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - components:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/{page_id}/custom_code\n  method: get\n  operationId: get-page-custom-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom_code:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/{page_id}/custom_code\n  method: delete\n  operationId: delete-page-custom-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/{page_id}/custom_code\n  method: put\n  operationId: add-custom-code-to-page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/custom_code\n  method: get\n  operationId: get-site-custom-code\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - custom_code:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/custom_code\n  method: delete\n  operationId: delete-site-custom-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/custom_code\n  method: put\n  operationId: add-custom-code-tosite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/registered_scripts\n  method:\
  \ get\n  operationId: get-scripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom_code:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/registered_scripts/hosted\n  method: post\n  operationId: post-hosted-script\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/registered_scripts/inline\n  method: post\n  operationId: post-inline-scripts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/custom_code/blocks\n  method: get\n  operationId: get-site-custom-code-blocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom_code:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/authorized_by\n  method: get\n  operationId: authorized_by\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - authorized_user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/introspect\n  method: get\n  operationId: introspect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace_id}/sites\n  method: post\n  operationId: create-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace_id_or_slug}/audit_logs\n  method: get\n  operationId: get-workspace-audit-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace_activity:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites\n  method: get\n  operationId: list-sites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sites:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}\n  method: get\n  operationId: get-site\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sites:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}\n\
  \  method: patch\n  operationId: update-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}\n  method: delete\n  operationId: delete-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/custom_domains\n  method: get\n  operationId: get-custom-domains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sites:read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /sites/{site_id}/publish\n  method: post\n  operationId: site-publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/redirects\n  method: get\n  operationId: get-redirects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sites:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/redirects\n  method: post\n  operationId: create-redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /sites/{site_id}/redirects/{redirect_id}\n  method: patch\n  operationId: update-redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/redirects/{redirect_id}\n  method: delete\n  operationId: delete-redirects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sites:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/plan\n  method: get\n  operationId: get-site-plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - sites:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/robots_txt\n  method: get\n  operationId: get-robots-txt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - site_config:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/robots_txt\n  method: put\n  operationId: replace-robots-txt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - site_config:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/robots_txt\n  method: patch\n  operationId: update-robots-txt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - site_config:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/robots_txt\n  method: delete\n  operationId: delete-robots-txt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - site_config:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/well_known\n  method: put\n  operationId: set-well-known\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - site_config:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/well_known\n\
  \  method: delete\n  operationId: delete-well-known\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - site_config:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/activity_logs\n  method: get\n  operationId: get-site-activity-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - site_activity:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/collections\n  method: get\n  operationId: list-collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/collections\n  method: post\n  operationId: create-collection\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}\n  method: get\n  operationId: collection-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}\n  method: delete\n  operationId: delete-collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/fields\n  method: post\n\
  \  operationId: create-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/fields/{field_id}\n  method: patch\n  operationId: update-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/fields/{field_id}\n  method: delete\n  operationId: delete-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items\n  method: get\n  operationId: list-collection-items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/items\n  method: post\n  operationId: create-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items\n  method: patch\n  operationId: update-items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items\n  method: delete\n  operationId: delete-items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/live\n  method: get\n  operationId: list-collection-items-live\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/items/live\n  method: post\n  operationId: create-item-live\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/live\n  method: patch\n  operationId: update-items-live\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/live\n  method: delete\n  operationId: delete-items-live\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/bulk\n  method: post\n  operationId: create-items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/{item_id}\n  method: get\n  operationId: Get-Item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/items/{item_id}\n  method: patch\n  operationId: update-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/{item_id}\n  method: delete\n  operationId: delete-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/{item_id}/live\n  method: get\n  operationId: get-item-live\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cms:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/items/{item_id}/live\n  method: patch\n  operationId: update-item-live\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/{item_id}/live\n  method: delete\n  operationId: delete-item-live\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}/items/publish\n  method: post\n  operationId: publish-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cms:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/comments\n  method: get\n  operationId: list-comment-threads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - comments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/comments/{comment_thread_id}\n  method: get\n  operationId: get-comment-thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - comments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/comments/{comment_thread_id}/replies\n  method: get\n  operationId: list-comment-replies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - comments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/pages\n  method: get\n  operationId: list-pages\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - page:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/{page_id}\n  method: get\n  operationId: get-page-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - page:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/{page_id}\n  method: put\n  operationId: update-page-settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - page:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/{page_id}/dom\n  method: get\n  operationId: get-static-content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - page:read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /pages/{page_id}/dom\n  method: post\n  operationId: update-static-content\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - page:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/components\n  method: get\n  operationId: list-components\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - components:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components/{component_id}/dom\n  method: get\n  operationId: get-component-content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - components:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components/{component_id}/dom\n\
  \  method: post\n  operationId: update-component-content\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - components:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/components/{component_id}/properties\n  method: get\n  operationId: get-component-properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - components:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/components/{component_id}/properties\n  method: post\n  operationId: update-component-properties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - components:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/{page_id}/custom_code\n  method: get\n  operationId: get-page-custom-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom_code:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/{page_id}/custom_code\n  method: delete\n  operationId: delete-page-custom-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/{page_id}/custom_code\n  method: put\n  operationId: add-custom-code-to-page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/custom_code\n  method: get\n  operationId: get-site-custom-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom_code:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site_id}/custom_code\n  method: delete\n  operationId: delete-site-custom-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site_id}/custom_code\n  method: put\n  operationId: add-custom-code-tosite\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - custom_code:write\n    audienc\n\n# --- truncated at 32 KB (68 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/agentic-access/webflow-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/agentic-access/webflow-agentic-access.yml
summary_line: 212 operations · 116 acting
tags:
- CMS
- Ecommerce
- No-Code
- Web Development
---
