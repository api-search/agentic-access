---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 41
api_specs:
- filename: reputation-asset-library-api-openapi.yml
  format: yaml
  label: Reputation Asset Library API
  slug: reputation-asset-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-asset-library-api-openapi.yml
- filename: reputation-authorize-api-openapi.yml
  format: yaml
  label: Reputation Authorize API
  slug: reputation-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-authorize-api-openapi.yml
- filename: reputation-categories-api-openapi.yml
  format: yaml
  label: Reputation Categories API
  slug: reputation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-categories-api-openapi.yml
- filename: reputation-credentials-api-openapi.yml
  format: yaml
  label: Reputation Credentials API
  slug: reputation-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-credentials-api-openapi.yml
- filename: reputation-listing-audits-api-openapi.yml
  format: yaml
  label: Reputation Listing Audits API
  slug: reputation-listing-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-listing-audits-api-openapi.yml
- filename: reputation-locations-api-openapi.yml
  format: yaml
  label: Reputation Locations API
  slug: reputation-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-locations-api-openapi.yml
- filename: reputation-metrics-api-openapi.yml
  format: yaml
  label: Reputation Metrics API
  slug: reputation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-metrics-api-openapi.yml
- filename: reputation-reports-api-openapi.yml
  format: yaml
  label: Reputation Reports API
  slug: reputation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reports-api-openapi.yml
- filename: reputation-requests-api-openapi.yml
  format: yaml
  label: Reputation Requests API
  slug: reputation-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-requests-api-openapi.yml
- filename: reputation-reviews-api-openapi.yml
  format: yaml
  label: Reputation Reviews API
  slug: reputation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reviews-api-openapi.yml
- filename: reputation-rich-content-api-openapi.yml
  format: yaml
  label: Reputation Rich Content API
  slug: reputation-rich-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-rich-content-api-openapi.yml
- filename: reputation-summary-api-openapi.yml
  format: yaml
  label: Reputation Summary API
  slug: reputation-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-summary-api-openapi.yml
- filename: reputation-surveys-api-openapi.yml
  format: yaml
  label: Reputation Surveys API
  slug: reputation-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-surveys-api-openapi.yml
- filename: reputation-tenants-api-openapi.yml
  format: yaml
  label: Reputation Tenants API
  slug: reputation-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tenants-api-openapi.yml
- filename: reputation-tickets-api-openapi.yml
  format: yaml
  label: Reputation Tickets API
  slug: reputation-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tickets-api-openapi.yml
- filename: reputation-users-api-openapi.yml
  format: yaml
  label: Reputation Users API
  slug: reputation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-users-api-openapi.yml
consequence_counts:
  physical: 2
  read: 41
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Reputation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/requests/send-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/requests/send-sms
operation_count: 67
overview: 'Reputation exposes 67 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read, 24 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reputation
provider_slug: reputation
slug: reputation-agentic-access
source_filename: reputation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/reputation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 67\n  by_action_class:\n    acting: 26\n    connected: 41\n  by_consequence:\n    write: 24\n    read: 41\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/asset-library/upload/image\n  method: post\n  operationId: post_asset_library_upload_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/asset-library/upload/image/url\n  method: post\n  operationId:\
  \ post_asset_library_upload_image_url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/authorize\n  method: post\n  operationId: post_authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/categories\n  method: get\n  operationId: get_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/credentials/oauth\n  method: get\n  operationId: get_credentials_oauth\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/listing-audits\n  method: get\n  operationId: get_listing_audits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/locations\n  method: get\n  operationId: get_locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/locations\n  method: post\n  operationId: post_locations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/locations-search\n  method: get\n  operationId: get_locations_search\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/locations-search\n  method: post\n  operationId: post_locations_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/locations-faceted-search\n  method: get\n  operationId: get_locations_faceted_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/locations/{locationID}\n  method: get\n  operationId: get_locations_locationID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/locations/{locationID}\n\
  \  method: delete\n  operationId: delete_locations_locationID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/locations/{locationID}/opt-out\n  method: put\n  operationId: put_locations_locationID_opt_out\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/locations/{locationID}/opt-in\n  method: put\n  operationId: put_locations_locationID_opt_in\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/locations/{locationID}/addPage\n  method: post\n  operationId: post_locations_locationID_addPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/location-attribute-definitions\n  method: get\n  operationId: get_location_attribute_definitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/locations-duplicate\n  method: get\n  operationId: get_locations_duplicate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/metrics\n\
  \  method: get\n  operationId: get_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/page-metrics\n  method: get\n  operationId: get_page_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/post-metrics\n  method: get\n  operationId: get_post_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/aggregate-page-metrics\n  method: get\n  operationId: get_aggregate_page_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/aggregate-post-metrics\n  method: get\n  operationId: get_aggregate_post_metrics\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reports/{reportID}/export\n  method: put\n  operationId: put_reports_reportID_export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/request-urls\n  method: get\n  operationId: get_request_urls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/requests/metrics\n  method: get\n  operationId: get_requests_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/requests/request-urls\n  method: get\n  operationId: get_requests_request_urls\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/requests/send-email\n  method: post\n  operationId: post_requests_send_email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/requests/send-sms\n  method: post\n  operationId: post_requests_send_sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/requests/unsubscribe-email\n\
  \  method: post\n  operationId: post_requests_unsubscribe_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/requests/unsubscribe-phone\n  method: post\n  operationId: post_requests_unsubscribe_phone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/requests/unsubscribes\n  method: get\n  operationId: get_requests_unsubscribes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/requests/templates\n  method:\
  \ get\n  operationId: get_requests_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews\n  method: get\n  operationId: get_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews/{reviewID}/responses\n  method: get\n  operationId: get_reviews_reviewID_responses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews/{reviewID}/respond\n  method: post\n  operationId: post_reviews_reviewID_respond\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v3/reviews3\n  method: get\n  operationId: get_reviews3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews3/{reviewID}/responses\n  method: get\n  operationId: get_reviews3_reviewID_responses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews3/{reviewID}/respond\n  method: post\n  operationId: post_reviews3_reviewID_respond\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/rich-content/faqs\n  method: get\n  operationId: get_rich_content_faqs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/rich-content/faqs/{faqId}\n  method: get\n  operationId: get_rich_content_faqs_faqId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/rich-content/menus\n  method: get\n  operationId: get_rich_content_menus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/rich-content/products\n  method: get\n  operationId: get_rich_content_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/summary\n  method: get\n  operationId: get_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v3/survey-results\n  method: get\n  operationId: get_survey_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/survey-results\n  method: post\n  operationId: post_survey_results\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/survey-results/{surveyID}\n  method: get\n  operationId: get_survey_results_surveyID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/surveys3-templates\n  method: get\n  operationId: get_surveys3_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/surveys-link\n  method: post\n  operationId: post_surveys_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/surveys2-results\n  method: get\n  operationId: get_surveys2_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/surveys2-results\n  method: post\n  operationId: post_surveys2_results\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v3/surveys2-results/create-url-from-encrypted\n  method: post\n  operationId: post_surveys2_results_create_url_from_encrypted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/surveys3-results/{surveyID}\n  method: get\n  operationId: get_surveys3_results_surveyID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/surveys3-results\n  method: post\n  operationId: post_surveys3_results\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v3/tenants\n  method: get\n  operationId: get_tenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/tenants\n  method: post\n  operationId: post_tenants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/tenants/{tenantID}\n  method: get\n  operationId: get_tenants_tenantID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/tenants/{tenantID}/pause\n  method: put\n  operationId: put_tenants_tenantID_pause\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/tenants/{tenantID}/unpause\n  method: put\n  operationId: put_tenants_tenantID_unpause\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/tickets\n  method: get\n  operationId: get_tickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/tickets\n  method: post\n  operationId: post_tickets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/ticket-queues\n  method: get\n  operationId: get_ticket_queues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ticket-stages\n  method: get\n  operationId: get_ticket_stages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ticket-types\n  method: get\n  operationId: get_ticket_types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/users\n  method: get\n  operationId: get_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/users\n\
  \  method: post\n  operationId: post_users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/users/{userID}\n  method: get\n  operationId: get_users_userID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/agentic-access/reputation-agentic-access.yml
summary_line: 67 operations · 26 acting
tags:
- Reputation Management
- Online Reviews
- Business Listings
- Surveys
- Social Listening
- Competitive Intelligence
- Customer Experience
- Local SEO
---
