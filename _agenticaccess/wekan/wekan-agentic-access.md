---
acting_count: 163
action_class_counts:
  acting: 163
  connected: 116
api_specs:
- filename: wekan-attachments-api-openapi.yml
  format: yaml
  label: WeKan Attachments API
  slug: wekan-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-attachments-api-openapi.yml
- filename: wekan-attachmentstoragesettings-api-openapi.yml
  format: yaml
  label: WeKan Attachment Storage Settings API
  slug: wekan-attachmentstoragesettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-attachmentstoragesettings-api-openapi.yml
- filename: wekan-boards-api-openapi.yml
  format: yaml
  label: WeKan Boards API
  slug: wekan-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-boards-api-openapi.yml
- filename: wekan-cardcomments-api-openapi.yml
  format: yaml
  label: WeKan Card Comments API
  slug: wekan-cardcomments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-cardcomments-api-openapi.yml
- filename: wekan-cards-api-openapi.yml
  format: yaml
  label: WeKan Cards API
  slug: wekan-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-cards-api-openapi.yml
- filename: wekan-checklists-api-openapi.yml
  format: yaml
  label: WeKan Checklists API
  slug: wekan-checklists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-checklists-api-openapi.yml
- filename: wekan-dependencies-api-openapi.yml
  format: yaml
  label: WeKan Dependencies API
  slug: wekan-dependencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-dependencies-api-openapi.yml
- filename: wekan-integrations-api-openapi.yml
  format: yaml
  label: WeKan Integrations API
  slug: wekan-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-integrations-api-openapi.yml
- filename: wekan-lists-api-openapi.yml
  format: yaml
  label: WeKan Lists API
  slug: wekan-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-lists-api-openapi.yml
- filename: wekan-login-api-openapi.yml
  format: yaml
  label: WeKan Login API
  slug: wekan-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-login-api-openapi.yml
- filename: wekan-org-api-openapi.yml
  format: yaml
  label: WeKan Org API
  slug: wekan-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-org-api-openapi.yml
- filename: wekan-organizations-api-openapi.yml
  format: yaml
  label: WeKan Organizations API
  slug: wekan-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-organizations-api-openapi.yml
- filename: wekan-problems-api-openapi.yml
  format: yaml
  label: WeKan Problems API
  slug: wekan-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-problems-api-openapi.yml
- filename: wekan-rules-api-openapi.yml
  format: yaml
  label: WeKan Rules API
  slug: wekan-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-rules-api-openapi.yml
- filename: wekan-settings-api-openapi.yml
  format: yaml
  label: WeKan Settings API
  slug: wekan-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-settings-api-openapi.yml
- filename: wekan-swimlanes-api-openapi.yml
  format: yaml
  label: WeKan Swimlanes API
  slug: wekan-swimlanes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-swimlanes-api-openapi.yml
- filename: wekan-team-api-openapi.yml
  format: yaml
  label: WeKan Team API
  slug: wekan-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-team-api-openapi.yml
- filename: wekan-teams-api-openapi.yml
  format: yaml
  label: WeKan Teams API
  slug: wekan-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-teams-api-openapi.yml
- filename: wekan-users-api-openapi.yml
  format: yaml
  label: WeKan Users API
  slug: wekan-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-users-api-openapi.yml
- filename: wekan-checklist-items-api-openapi.yml
  format: yaml
  label: WeKan Checklist Items API
  slug: wekan-checklist-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-checklist-items-api-openapi.yml
- filename: wekan-custom-fields-api-openapi.yml
  format: yaml
  label: WeKan Custom Fields API
  slug: wekan-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-custom-fields-api-openapi.yml
- filename: wekan-event-log-api-openapi.yml
  format: yaml
  label: WeKan Event Log API
  slug: wekan-event-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wekan/openapi/wekan-event-log-api-openapi.yml
consequence_counts:
  physical: 1
  read: 116
  safety-critical: 1
  write: 161
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wekan Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/boards/{board}/domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/boards/{board}/cardFieldOrder
operation_count: 279
overview: 'WeKan exposes 279 API operations that an AI agent could call, of which 163 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 116 read, 161 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WeKan
provider_slug: wekan
slug: wekan-agentic-access
source_filename: wekan-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/wekan-meteor3-openapi.yml, openapi/wekan-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 279\n  by_action_class:\n    acting: 163\n    connected: 116\n  by_consequence:\n    write: 161\n    read: 116\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /users/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/register\n  method: post\n  operationId:\
  \ register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/attachment-settings\n  method: get\n  operationId: get_attachment_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/attachment-settings\n  method: put\n  operationId: update_attachment_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/domains\n  method: get\n  operationId: get_admin_domains\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/orgs\n  method: get\n  operationId: get_admin_orgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/orgs/{org}/features\n  method: put\n  operationId: update_admin_org_features\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/orgs/features\n  method: put\n  operationId: update_all_admin_org_features\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/teams\n  method: get\n  operationId: get_admin_teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/teams/{team}/features\n  method: put\n  operationId: update_admin_team_features\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/teams/features\n  method: put\n  operationId: update_all_admin_team_features\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/attachments/{attachment}/export\n  method: get\n  operationId: exportJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/checklists\n  method: get\n  operationId: get_board_card_checklists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/checklists\n  method: post\n  operationId: post_board_card_checklists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/checklists/{checklist}\n\
  \  method: get\n  operationId: get_board_card_checklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/checklists/{checklist}\n  method: delete\n  operationId: delete_board_card_checklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/checklists/{checklist}/items\n  method: post\n  operationId: post_board_card_checklist_items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/boards/{board}/cards/{card}/checklists/{checklist}/items/{item}\n  method: get\n  operationId: get_board_card_checklist_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/checklists/{checklist}/items/{item}\n  method: put\n  operationId: put_board_card_checklist_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/checklists/{checklist}/items/{item}\n  method: delete\n  operationId: delete_board_card_checklist_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/comments\n  method: get\n  operationId: get_board_card_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/comments\n  method: post\n  operationId: post_board_card_comments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/comments/{comment}\n  method: get\n  operationId: get_board_card_comment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/comments/{comment}\n  method: delete\n  operationId: delete_board_card_comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/dependencies\n  method: get\n  operationId: get_card_dependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards/{card}/dependencies\n  method: post\n  operationId: new_card_dependency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/dependencies/{target}\n  method: put\n  operationId: edit_card_dependency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/{card}/dependencies/{target}\n  method: delete\n  operationId: delete_card_dependency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/bulk\n  method: delete\n  operationId: delete_board_cards_bulk\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cards/labels\n  method: post\n  operationId: post_board_cards_labels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/cardsByCustomField/{customField}/{customFieldValue}\n  method: get\n  operationId: get_board_customFieldValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/cards_count\n  method: get\n  operationId: get_board_cards_count\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/custom-fields\n  method: get\n  operationId: get_board_custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/custom-fields\n  method: post\n  operationId: post_board_custom-fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/custom-fields/{customField}\n  method: get\n  operationId: get_board_customField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/boards/{board}/custom-fields/{customField}\n  method: put\n  operationId: put_board_customField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/custom-fields/{customField}\n  method: delete\n  operationId: delete_board_customField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/custom-fields/{customField}/dropdown-items\n  method: post\n  operationId: post_board_customField_dropdown-items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/custom-fields/{customField}/dropdown-items/{dropdownItem}\n  method: put\n  operationId: put_board_customField_dropdownItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/custom-fields/{customField}/dropdown-items/{dropdownItem}\n  method: delete\n  operationId: delete_board_customField_dropdownItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/dependencies\n  method: get\n  operationId: get_board_dependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/export\n  method: get\n  operationId: exportJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/export/{format}\n  method: get\n  operationId: exportExternal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/export/csv\n  method: get\n  operationId: exportCSV/TSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/boards/{board}/export/kanboard\n  method: get\n  operationId: exportKanboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/exportExcel\n  method: get\n  operationId: exportExcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/exportPDF\n  method: get\n  operationId: exportBoardPDF\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/exportZip\n  method: get\n  operationId: exportZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/integrations\n  method: get\n  operationId: get_board_integrations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/integrations\n  method: post\n  operationId: post_board_integrations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/integrations/{int}\n  method: get\n  operationId: get_board_int\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/integrations/{int}\n  method: put\n  operationId: put_board_int\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/integrations/{int}\n  method: delete\n  operationId: delete_board_int\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/integrations/{int}/activities\n  method: delete\n  operationId: delete_board_int_activities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/integrations/{int}/activities\n  method: post\n  operationId: post_board_int_activities\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists\n  method: get\n  operationId: get_board_lists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/lists\n  method: post\n  operationId: post_board_lists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}\n  method: get\n  operationId: get_board_list\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/lists/{list}\n  method: put\n  operationId: put_board_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}\n  method: delete\n  operationId: delete_board_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards\n  method: get\n  operationId: get_board_list_cards\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/lists/{list}/cards\n  method: post\n  operationId: post_board_list_cards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}\n  method: get\n  operationId: get_board_list_card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/lists/{list}/cards/{card}\n  method: put\n  operationId: put_board_list_card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}\n  method: delete\n  operationId: delete_board_list_card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/archive\n  method: post\n  operationId: post_board_list_card_archive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/assignees/{assignee}\n  method: post\n  operationId: post_board_list_card_assignee\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/assignees/{assignee}\n  method: delete\n  operationId: delete_board_list_card_assignee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/copy\n  method: post\n  operationId: post_board_list_card_copy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/customFields/{customField}\n  method: post\n  operationId: post_board_list_card_customField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/exportExcel\n  method: get\n  operationId: exportExcelCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/lists/{list}/cards/{card}/exportPDF\n  method: get\n  operationId: exportExcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/boards/{board}/lists/{list}/cards/{card}/members/{member}\n  method: post\n  operationId: post_board_list_card_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/members/{member}\n  method: delete\n  operationId: delete_board_list_card_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/{card}/unarchive\n  method: post\n  operationId: post_board_list_card_unarchive\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards/bulk\n  method: post\n  operationId: post_board_list_cards_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/cards_count\n  method: get\n  operationId: get_board_list_cards_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/lists/{list}/copy\n  method: post\n  operationId: post_board_list_copy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/lists/{list}/move\n  method: post\n  operationId: post_board_list_move\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/members/{user}/add\n  method: post\n  operationId: post_board_user_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/boards/{board}/members/{user}/remove\n  method: post\n  operationId: post_board_user_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/rules\n  method: get\n  operationId: get_board_rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/rules\n  method: post\n  operationId: new_board_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/boards/{board}/rules/{rule}\n  method: get\n  operationId: get_board_rule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/rules/{rule}\n  method: put\n  operationId: edit_board_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/rules/{rule}\n  method: delete\n  operationId: delete_board_rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/swimlanes\n\
  \  method: get\n  operationId: get_board_swimlanes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/swimlanes\n  method: post\n  operationId: post_board_swimlanes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/swimlanes/{swimlane}\n  method: get\n  operationId: get_board_swimlane\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/swimlanes/{swimlane}\n  method: put\n  operationId: put_board_swimlane\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/swimlanes/{swimlane}\n  method: delete\n  operationId: delete_board_swimlane\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/swimlanes/{swimlane}/cards\n  method: get\n  operationId: get_board_swimlane_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/boards/{board}/swimlanes/{swimlane}/copy\n  method: post\n  operationId: post_board_swimlane_copy\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/boards/{board}/swimlanes/{swimlane}/move\n  method: post\n  operationId: post_board_swimlane_move\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cards/{card}\n  method: get\n  operationId: get_card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/createtoken/{user}\n  method: post\n  operationId: post_user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deletetoken\n  method: post\n  operationId: post_deletetoken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/import/zip\n  method: post\n  operationId: importZip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/settings\n  method: get\n  operationId: get_global_settings\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/settings\n  method: put\n  operationId: update_global_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/user\n  method: get\n  operationId: get_user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/cards\n  method: get\n  operationId: get_user_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users\n  method: get\n  operationId: get_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (84 KB total) ---\n# Full source: https://artifacts.apis.io/wekan/agentic-access/wekan-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/wekan/agentic-access/wekan-agentic-access.yml
summary_line: 279 operations · 163 acting · 1 human-in-the-loop
tags:
- Company
---
