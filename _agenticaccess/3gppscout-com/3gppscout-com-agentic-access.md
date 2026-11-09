---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 66
api_specs:
- filename: 3gppscout-com-analysis-api-openapi.yml
  format: yaml
  label: 3GPP Scout Analysis API
  slug: 3gppscout-com-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-analysis-api-openapi.yml
- filename: 3gppscout-com-documents-api-openapi.yml
  format: yaml
  label: 3GPP Scout Documents API
  slug: 3gppscout-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-documents-api-openapi.yml
- filename: 3gppscout-com-follow-api-openapi.yml
  format: yaml
  label: 3GPP Scout Follow API
  slug: 3gppscout-com-follow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-follow-api-openapi.yml
- filename: 3gppscout-com-images-api-openapi.yml
  format: yaml
  label: 3GPP Scout Images API
  slug: 3gppscout-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-images-api-openapi.yml
- filename: 3gppscout-com-meetings-api-openapi.yml
  format: yaml
  label: 3GPP Scout Meetings API
  slug: 3gppscout-com-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-meetings-api-openapi.yml
- filename: 3gppscout-com-news-api-openapi.yml
  format: yaml
  label: 3GPP Scout News API
  slug: 3gppscout-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-news-api-openapi.yml
- filename: 3gppscout-com-organizations-api-openapi.yml
  format: yaml
  label: 3GPP Scout Organizations API
  slug: 3gppscout-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-organizations-api-openapi.yml
- filename: 3gppscout-com-positions-api-openapi.yml
  format: yaml
  label: 3GPP Scout Positions API
  slug: 3gppscout-com-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-positions-api-openapi.yml
- filename: 3gppscout-com-rfcs-api-openapi.yml
  format: yaml
  label: 3GPP Scout Rfcs API
  slug: 3gppscout-com-rfcs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-rfcs-api-openapi.yml
- filename: 3gppscout-com-search-api-openapi.yml
  format: yaml
  label: 3GPP Scout Search API
  slug: 3gppscout-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-search-api-openapi.yml
- filename: 3gppscout-com-sections-api-openapi.yml
  format: yaml
  label: 3GPP Scout Sections API
  slug: 3gppscout-com-sections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-sections-api-openapi.yml
- filename: 3gppscout-com-system-api-openapi.yml
  format: yaml
  label: 3GPP Scout System API
  slug: 3gppscout-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-system-api-openapi.yml
- filename: 3gppscout-com-tdocs-api-openapi.yml
  format: yaml
  label: 3GPP Scout Tdocs API
  slug: 3gppscout-com-tdocs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3gppscout-com/openapi/3gppscout-com-tdocs-api-openapi.yml
consequence_counts:
  read: 66
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 3Gppscout Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 82
overview: '3GPP Scout exposes 82 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 66 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 3GPP Scout
provider_slug: 3gppscout-com
slug: 3gppscout-com-agentic-access
source_filename: 3gppscout-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/3gppscout-com-openapi.json, openapi/api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    connected: 66\n    acting: 16\n  by_consequence:\n    read: 66\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/text\n  method: post\n  operationId: search_text_search_text_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /search/images\n  method: post\n  operationId: search_images_search_images_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/combined\n  method: post\n  operationId: search_combined_search_combined_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: get\n  operationId: list_documents_documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}\n  method: get\n  operationId: get_document_documents__document_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections\n  method: get\n  operationId:\
  \ get_sections_sections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/toc\n  method: get\n  operationId: list_sections_sections_toc_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/window\n  method: get\n  operationId: get_section_window_sections_window_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/batch\n  method: post\n  operationId: get_sections_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/{doc_number}/{version}/{image_index}\n  method: get\n  operationId: get_image_images__doc_number___version___image_index__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/search\n  method: post\n  operationId: search_tdocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfcs/search\n  method: post\n  operationId: search_ietf_rfcs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfcs/{rfc_number}\n  method: get\n  operationId: get_rfc_section\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/{tdoc_id}\n  method: get\n  operationId: get_tdoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /tdocs/batch\n  method: post\n  operationId: get_tdocs_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/{tdoc_id}/fetch\n  method: post\n  operationId: fetch_tdoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs\n  method: get\n  operationId: list_tdocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings\n  method: get\n  operationId: list_meetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meeting_id}\n  method: get\n  operationId: get_meeting\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meeting_id}/decisions\n  method: get\n  operationId: list_meeting_decisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId: resolve_organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}\n  method: get\n  operationId: get_organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions\n  method: get\n  operationId: get_company_positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/search\n\
  \  method: post\n  operationId: search_positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/search\n  method: get\n  operationId: search_news\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows/resolve\n  method: post\n  operationId: find_topics_to_follow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows\n  method: get\n  operationId: list_followed_topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows\n  method: post\n  operationId: follow_topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}\n  method: patch\n  operationId: update_followed_topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}\n  method: delete\n  operationId: unfollow_topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}/updates\n  method: get\n  operationId: get_followed_topic_updates\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows/{follow_id}/updates/{event_id}/not-relevant\n  method: post\n  operationId: mark_update_not_relevant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}/feedback/{feedback_id}\n  method: delete\n  operationId: undo_update_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}/updates/{event_id}\n  method: get\n  operationId:\
  \ get_followed_topic_update\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/proposal\n  method: post\n  operationId: compare_proposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/proposal/{comparison_id}\n  method: get\n  operationId: get_proposal_comparison\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows/patent\n  method: post\n  operationId: follow_patent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/lookup\n  method: get\n  operationId: reference_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simulation-results\n  method: get\n  operationId: find_simulation_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/check-message\n  method: post\n  operationId: check_message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/text\n  method: post\n  operationId: search_text_search_text_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/images\n  method: post\n  operationId: search_images_search_images_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/combined\n  method: post\n  operationId: search_combined_search_combined_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: get\n  operationId: list_documents_documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}\n  method: get\n  operationId: get_document_documents__document_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections\n  method: get\n  operationId: get_sections_sections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/toc\n  method: get\n  operationId: list_sections_sections_toc_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/window\n  method: get\n  operationId: get_section_window_sections_window_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /sections/batch\n  method: post\n  operationId: get_sections_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/{doc_number}/{version}/{image_index}\n  method: get\n  operationId: get_image_images__doc_number___version___image_index__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/search\n  method: post\n  operationId: search_tdocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfcs/search\n  method: post\n  operationId: search_ietf_rfcs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfcs/{rfc_number}\n  method: get\n  operationId:\
  \ get_rfc_section\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/{tdoc_id}\n  method: get\n  operationId: get_tdoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/batch\n  method: post\n  operationId: get_tdocs_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs/{tdoc_id}/fetch\n  method: post\n  operationId: fetch_tdoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tdocs\n  method: get\n  operationId: list_tdocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /meetings\n  method: get\n  operationId: list_meetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meeting_id}\n  method: get\n  operationId: get_meeting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meeting_id}/decisions\n  method: get\n  operationId: list_meeting_decisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId: resolve_organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}\n  method: get\n  operationId: get_organization\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions\n  method: get\n  operationId: get_company_positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/search\n  method: post\n  operationId: search_positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/search\n  method: get\n  operationId: search_news\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows/resolve\n  method: post\n  operationId: find_topics_to_follow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /follows\n  method: get\n  operationId: list_followed_topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows\n  method: post\n  operationId: follow_topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}\n  method: patch\n  operationId: update_followed_topic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}\n  method: delete\n  operationId: unfollow_topic\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}/updates\n  method: get\n  operationId: get_followed_topic_updates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows/{follow_id}/updates/{event_id}/not-relevant\n  method: post\n  operationId: mark_update_not_relevant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}/feedback/{feedback_id}\n  method: delete\n  operationId: undo_update_feedback\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /follows/{follow_id}/updates/{event_id}\n  method: get\n  operationId: get_followed_topic_update\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/proposal\n  method: post\n  operationId: compare_proposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/proposal/{comparison_id}\n  method: get\n  operationId: get_proposal_comparison\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /follows/patent\n  method: post\n  operationId: follow_patent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference/lookup\n  method: get\n  operationId: reference_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simulation-results\n  method: get\n  operationId: find_simulation_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference/check-message\n  method: post\n  operationId: check_message\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/3gppscout-com/agentic-access/3gppscout-com-agentic-access.yml
summary_line: 82 operations · 16 acting
tags:
- 3GPP
- Standards
- Search
- Artificial Intelligence
---
