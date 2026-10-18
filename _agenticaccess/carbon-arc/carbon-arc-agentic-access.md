---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 65
api_specs:
- filename: carbon-arc-block-api-openapi.yml
  format: yaml
  label: Carbon Arc Block API
  slug: carbon-arc-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-block-api-openapi.yml
- filename: carbon-arc-bucket-access-api-openapi.yml
  format: yaml
  label: Carbon Arc Bucket Access API
  slug: carbon-arc-bucket-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-bucket-access-api-openapi.yml
- filename: carbon-arc-catalog-api-openapi.yml
  format: yaml
  label: Carbon Arc Catalog API
  slug: carbon-arc-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-catalog-api-openapi.yml
- filename: carbon-arc-clients-api-openapi.yml
  format: yaml
  label: Carbon Arc Clients API
  slug: carbon-arc-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-clients-api-openapi.yml
- filename: carbon-arc-data-library-api-openapi.yml
  format: yaml
  label: Carbon Arc Data Library API
  slug: carbon-arc-data-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-data-library-api-openapi.yml
- filename: carbon-arc-explore-use-cases-api-openapi.yml
  format: yaml
  label: Carbon Arc Explore Use Cases API
  slug: carbon-arc-explore-use-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-explore-use-cases-api-openapi.yml
- filename: carbon-arc-framework-api-openapi.yml
  format: yaml
  label: Carbon Arc Framework API
  slug: carbon-arc-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-framework-api-openapi.yml
- filename: carbon-arc-ontology-api-openapi.yml
  format: yaml
  label: Carbon Arc Ontology API
  slug: carbon-arc-ontology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-ontology-api-openapi.yml
- filename: carbon-arc-ontology-internal-api-openapi.yml
  format: yaml
  label: Carbon Arc Ontology Internal API
  slug: carbon-arc-ontology-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-ontology-internal-api-openapi.yml
- filename: carbon-arc-polaris-api-openapi.yml
  format: yaml
  label: Carbon Arc Polaris API
  slug: carbon-arc-polaris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-polaris-api-openapi.yml
- filename: carbon-arc-prisms-api-openapi.yml
  format: yaml
  label: Carbon Arc Prisms API
  slug: carbon-arc-prisms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-prisms-api-openapi.yml
- filename: carbon-arc-public-api-openapi.yml
  format: yaml
  label: Carbon Arc Public API
  slug: carbon-arc-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-public-api-openapi.yml
- filename: carbon-arc-research-api-openapi.yml
  format: yaml
  label: Carbon Arc Research API
  slug: carbon-arc-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-research-api-openapi.yml
- filename: carbon-arc-tracking-api-openapi.yml
  format: yaml
  label: Carbon Arc Tracking API
  slug: carbon-arc-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-tracking-api-openapi.yml
- filename: carbon-arc-transcripts-api-openapi.yml
  format: yaml
  label: Carbon Arc Transcripts API
  slug: carbon-arc-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/openapi/carbon-arc-transcripts-api-openapi.yml
consequence_counts:
  physical: 3
  read: 65
  safety-critical: 3
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Carbon Arc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/bucket-access/datasets/{dataset_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/polaris/datasets/{dataset_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/polaris/reset-credentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/clients/me/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/framework/buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/transcripts/{transcript_id}/purchase
operation_count: 92
overview: 'Carbon Arc exposes 92 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 65 read, 21 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Carbon Arc
provider_slug: carbon-arc
slug: carbon-arc-agentic-access
source_filename: carbon-arc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/carbon-arc-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 92\n  by_action_class:\n    connected: 65\n    acting: 27\n  by_consequence:\n    read: 65\n    physical: 3\n    write: 21\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v2/ontology/entities/{entity_id}\n  method: get\n  operationId: get_entity_by_id_v2_ontology_entities__entity_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/entity/{entity_id}/insights\n  method: get\n  operationId: insights_for_entity_v2_ontology_entity__entity_id__insights_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insight/{insight_id}/entities\n  method: get\n  operationId: entities_for_insight_v2_ontology_insight__insight_id__entities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/entity-map\n  method: get\n  operationId: get_entity_map_v2_ontology_entity_map_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/categories\n  method: get\n  operationId: get_categories_v2_ontology_categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/categories/{category_label}\n  method: get\n  operationId:\
  \ get_category_v2_ontology_categories__category_label__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/categories/{entity_id}/{entity_representation}\n  method: get\n  operationId: get_categories_from_entity_v2_ontology_categories__entity_id___entity_representation__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/subjects\n  method: get\n  operationId: get_subjects_v2_ontology_subjects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/subject/{subject_id}/insights\n  method: get\n  operationId: subject_insights_v2_ontology_subject__subject_id__insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/topic/{topic_id}/insights\n  method: get\n  operationId: topic_insights_v2_ontology_topic__topic_id__insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insight-map\n  method: get\n  operationId: get_insight_map_v2_ontology_insight_map_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insights\n  method: get\n  operationId: get_insights_list_v2_ontology_insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/all-insights\n  method: get\n  operationId: all_insights_v2_ontology_all_insights_get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insights/batch\n  method: post\n  operationId: get_insights_list_batch_v2_ontology_insights_batch_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/builder\n  method: get\n  operationId: get_builder_bootstrap_v2_ontology_builder_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insight-search-ids\n  method: get\n  operationId: insight_search_ids_v2_ontology_insight_search_ids_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insights/linked\n  method: get\n  operationId: linked_insight_ids_v2_ontology_insights_linked_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/insights/{insight_id}\n  method: get\n  operationId: insight_details_v2_ontology_insights__insight_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ontology/ontology-versions\n  method: get\n  operationId: get_ontology_versions_v2_ontology_ontology_versions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/clients/payments/balance-summary\n  method: get\n  operationId: get_client_balance_v2_clients_payments_balance_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/clients/me/orders\n\
  \  method: get\n  operationId: get_user_orders_v2_clients_me_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/clients/me/orders/{order_id}\n  method: get\n  operationId: get_user_order_v2_clients_me_orders__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/clients/me/orders/{order_id}\n  method: patch\n  operationId: update_user_order_display_name_v2_clients_me_orders__order_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/library/data\n  method:\
  \ get\n  operationId: get_data_identifiers_v2_library_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/data/{dataset_id}\n  method: get\n  operationId: get_data_identifier_information_v2_library_data__dataset_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/data/{dataset_id}/data-dictionary\n  method: get\n  operationId: get_data_dictionary_by_dataset_id_v2_library_data__dataset_id__data_dictionary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/data/{dataset_id}/tearsheet-pdf\n  method: get\n  operationId: get_tearsheet_pdf_by_dataset_id_v2_library_data__dataset_id__tearsheet_pdf_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/data/{dataset_id}/insights\n  method: get\n  operationId: get_insights_by_dataset_v2_library_data__dataset_id__insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/graph\n  method: get\n  operationId: get_graph_identifiers_v2_library_graph_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/graph/{graph_id}\n  method: get\n  operationId: get_graph_information_v2_library_graph__graph_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/schedule/export\n  method: get\n  operationId: export_cake_task_schedule_v2_library_schedule_export_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/library/schedule/{dataset_id}\n  method: get\n  operationId: get_cake_task_schedule_v2_library_schedule__dataset_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/block/datasets\n  method: get\n  operationId: list_block_datasets_v2_block_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/block/datasets/{dataset_id}/cuts\n  method: get\n  operationId: list_dataset_cuts_v2_block_datasets__dataset_id__cuts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/filters\n  method: post\n\
  \  operationId: framework_filters_v2_framework_filters_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/framework/filters/batch\n  method: post\n  operationId: framework_filters_batch_v2_framework_filters_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/framework/filters/{filter_key}/options\n  method: post\n  operationId: framework_filter_options_v2_framework_filters__filter_key__options_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/framework/metadata\n  method: post\n  operationId: collection_framework_metadata_v2_framework_metadata_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/framework/buy\n  method: post\n  operationId: create_framework_order_v2_framework_buy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/framework/{framework_id}/metadata\n  method: get\n  operationId: get_framework_metadata_by_id_v2_framework__framework_id__metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/{framework_id}/data\n  method: get\n  operationId: get_framework_data_v2_framework__framework_id__data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/{framework_id}/export\n  method: get\n  operationId: export_framework_data_v2_framework__framework_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/code/preview\n  method: post\n  operationId: preview_framework_code_v2_framework_code_preview_post\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/framework/{framework_id}/code\n  method: get\n  operationId: get_framework_code_v2_framework__framework_id__code_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/{framework_id}/panel-debias\n  method: get\n  operationId: get_panel_debias_framework_data_v2_framework__framework_id__panel_debias_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/{framework_id}/panel-debias-info\n  method: get\n  operationId: get_panel_debias_info_v2_framework__framework_id__panel_debias_info_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/framework-status\n  method: get\n  operationId: get_framework_data_status_v2_framework_framework_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/framework/{framework_id}/name\n  method: patch\n  operationId: update_framework_name_v2_framework__framework_id__name_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/access\n  method: get\n  operationId: check_catalog_access_v2_catalog_access_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/subscriptions\n  method: get\n  operationId: get_subscriptions_v2_catalog_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/assets\n  method: get\n  operationId: list_assets_v2_catalog_assets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/assets/admin\n  method: get\n  operationId: admin_list_assets_v2_catalog_assets_admin_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/assets/admin/{asset_id}\n  method: get\n  operationId: admin_get_asset_v2_catalog_assets_admin__asset_id__get\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/assets/{asset_id}\n  method: patch\n  operationId: admin_update_asset_v2_catalog_assets__asset_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/assets/{asset_id}\n  method: get\n  operationId: get_asset_v2_catalog_assets__asset_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/assets/{asset_id}/vote\n  method: post\n  operationId: toggle_vote_v2_catalog_assets__asset_id__vote_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/assets/{asset_id}/vote\n  method: get\n  operationId: get_vote_status_v2_catalog_assets__asset_id__vote_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/assets/{asset_id}/request-access\n  method: post\n  operationId: request_access_v2_catalog_assets__asset_id__request_access_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/clients\n  method: get\n  operationId: list_clients_v2_catalog_clients_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/clients\n  method: post\n  operationId: create_client_v2_catalog_clients_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/clients/{client_id}\n  method: get\n  operationId: get_client_v2_catalog_clients__client_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog/clients/{client_id}\n  method: patch\n  operationId: update_client_v2_catalog_clients__client_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/clients/{client_id}\n  method: delete\n  operationId: delete_client_v2_catalog_clients__client_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/catalog/clients/{client_id}/audit-log\n  method: get\n  operationId: get_client_audit_log_v2_catalog_clients__client_id__audit_log_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/polaris/datasets/{dataset_id}/example-table\n  method: get\n  operationId: get_example_table_v2_polaris_datasets__dataset_id__example_table_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transcripts\n  method: get\n  operationId: list_transcripts_v2_transcripts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transcripts/all\n  method: get\n  operationId: all_transcripts_v2_transcripts_all_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transcripts/entities\n  method: get\n  operationId: list_transcript_entities_v2_transcripts_entities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transcripts/regions\n  method: get\n  operationId: list_transcript_regions_v2_transcripts_regions_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transcripts/{transcript_id}\n  method: get\n  operationId: get_transcript_v2_transcripts__transcript_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transcripts/{transcript_id}/purchase\n  method: post\n  operationId: purchase_transcript_v2_transcripts__transcript_id__purchase_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transcripts/{transcript_id}/download\n  method: get\n  operationId: download_transcript_v2_transcripts__transcript_id__download_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prisms\n  method: get\n  operationId: list_prisms_v2_prisms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prisms/{prism_id}\n  method: get\n  operationId: get_prism_v2_prisms__prism_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/explore-use-cases/match\n  method: post\n  operationId: match_datasets_v2_explore_use_cases_match_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/research/case-studies\n  method: get\n  operationId: get_case_studies_v2_research_case_studies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/public-library/data-library\n  method: get\n  operationId: get_public_datalibrary_identifiers_v2_public_library_data_library_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/public-library/explore-data\n  method: get\n  operationId: get_public_explore_data_v2_public_library_explore_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tracking/events\n  method: post\n  operationId: track_capi_event_v2_tracking_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/public-prisms\n  method: get\n  operationId: get_prisms_page_v2_public_prisms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/polaris/onboard\n  method: post\n  operationId: onboard_client_v2_polaris_onboard_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/polaris/principals/{principal_name}\n  method: delete\n  operationId: offboard_client_v2_polaris_principals__principal_name__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/polaris/reset-credentials\n  method: post\n  operationId: reset_credentials_v2_polaris_reset_credentials_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/polaris/datasets/{dataset_id}/grant\n  method: post\n  operationId: grant_dataset_access_v2_polaris_datasets__dataset_id__grant_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/polaris/datasets/{dataset_id}/revoke\n  method: post\n  operationId: revoke_dataset_access_v2_polaris_datasets__dataset_id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/polaris/datasets/{dataset_id}/verify\n  method: post\n  operationId: verify_dataset_access_v2_polaris_datasets__dataset_id__verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/polaris/principals/{principal_name}/bulk-browse\n\
  \  method: post\n  operationId: assign_bulk_browse_v2_polaris_principals__principal_name__bulk_browse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/bucket-access/datasets/{dataset_id}/grant\n  method: post\n  operationId: grant_bucket_access_v2_bucket_access_datasets__dataset_id__grant_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/bucket-access/datasets/{dataset_id}/revoke\n  method: post\n  operationId: revoke_bucket_access_v2_bucket_access_datasets__dataset_id__revoke_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/bucket-access/datasets/{dataset_id}/verify\n  method: post\n  operationId: verify_bucket_access_v2_bucket_access_datasets__dataset_id__verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ontology/internal/entities\n  method: get\n  operationId: search_entities_v2_ontology_internal_entities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v2/ontology/internal/all-insights\n  method: get\n  operationId: all_insights_v2_ontology_internal_all_insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-arc/refs/heads/main/agentic-access/carbon-arc-agentic-access.yml
summary_line: 92 operations · 27 acting · 3 human-in-the-loop
tags:
- Artificial Intelligence
- Infrastructure
- Platform
- MLOps
- Enterprise
---
