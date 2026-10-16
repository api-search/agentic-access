---
acting_count: 142
action_class_counts:
  acting: 142
  connected: 135
api_specs:
- filename: trello-webhooks-asyncapi.yml
  format: yaml
  label: Trello Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/asyncapi/trello-webhooks-asyncapi.yml
- filename: trello-actions-api-openapi.yml
  format: yaml
  label: trello Actions API
  slug: trello-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-actions-api-openapi.yml
- filename: trello-boards-api-openapi.yml
  format: yaml
  label: trello Boards API
  slug: trello-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-boards-api-openapi.yml
- filename: trello-cards-api-openapi.yml
  format: yaml
  label: trello Cards API
  slug: trello-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-cards-api-openapi.yml
- filename: trello-checklists-api-openapi.yml
  format: yaml
  label: trello Checklists API
  slug: trello-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-checklists-api-openapi.yml
- filename: trello-labels-api-openapi.yml
  format: yaml
  label: trello Labels API
  slug: trello-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-labels-api-openapi.yml
- filename: trello-lists-api-openapi.yml
  format: yaml
  label: trello Lists API
  slug: trello-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-lists-api-openapi.yml
- filename: trello-members-api-openapi.yml
  format: yaml
  label: trello Members API
  slug: trello-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-members-api-openapi.yml
- filename: trello-notifications-api-openapi.yml
  format: yaml
  label: trello Notifications API
  slug: trello-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-notifications-api-openapi.yml
- filename: trello-organizations-api-openapi.yml
  format: yaml
  label: trello Organizations API
  slug: trello-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-organizations-api-openapi.yml
- filename: trello-plugins-api-openapi.yml
  format: yaml
  label: trello Plugins API
  slug: trello-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-plugins-api-openapi.yml
- filename: trello-search-api-openapi.yml
  format: yaml
  label: trello Search API
  slug: trello-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-search-api-openapi.yml
- filename: trello-tokens-api-openapi.yml
  format: yaml
  label: trello Tokens API
  slug: trello-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-tokens-api-openapi.yml
- filename: trello-webhooks-api-openapi.yml
  format: yaml
  label: trello Webhooks API
  slug: trello-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-webhooks-api-openapi.yml
- filename: trello-applications-api-openapi.yml
  format: yaml
  label: Trello Applications API
  slug: trello-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-applications-api-openapi.yml
- filename: trello-batch-api-openapi.yml
  format: yaml
  label: Trello Batch API
  slug: trello-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-batch-api-openapi.yml
- filename: trello-emoji-api-openapi.yml
  format: yaml
  label: Trello Emoji API
  slug: trello-emoji-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-emoji-api-openapi.yml
- filename: trello-enterprises-api-openapi.yml
  format: yaml
  label: Trello Enterprises API
  slug: trello-enterprises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-enterprises-api-openapi.yml
- filename: trello-custom-fields-api-openapi.yml
  format: yaml
  label: Trello Custom Fields API
  slug: trello-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-custom-fields-api-openapi.yml
consequence_counts:
  physical: 2
  read: 135
  safety-critical: 1
  write: 139
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Trello Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /boards/{id}/boardPlugins/{idPlugin}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /boards/{id}/memberships/{idMembership}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /enterprises/{id}/organizations
operation_count: 277
overview: 'Trello exposes 277 API operations that an AI agent could call, of which 142 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 135 read, 139 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trello
provider_slug: trello
slug: trello-agentic-access
source_filename: trello-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: generated\nsource: openapi/trello-actions-api-openapi.yml, openapi/trello-applications-api-openapi.yml,\n  openapi/trello-batch-api-openapi.yml, openapi/trello-boards-api-openapi.yml, openapi/trello-cards-api-openapi.yml,\n  openapi/trello-checklists-api-openapi.yml, openapi/trello-custom-fields-api-openapi.yml, openapi/trello-emoji-api-openapi.yml,\n  openapi/trello-enterprises-api-openapi.yml, openapi/trello-labels-api-openapi.yml, openapi/trello-lists-api-openapi.yml,\n  openapi/trello-members-api-openapi.yml, openapi/trello-notifications-api-openapi.yml, openapi/trello-organizations-api-openapi.yml,\n  openapi/trello-plugins-api-openapi.yml, openapi/trello-search-api-openapi.yml, openapi/trello-tokens-api-openapi.yml,\n  openapi/trello-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review\
  \ and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 277\n  by_action_class:\n    connected: 135\n    acting: 142\n  by_consequence:\n    read: 135\n    write: 139\n    physical: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /actions/{id}\n  method: get\n  operationId: getAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}\n  method: put\n  operationId: updateAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{id}\n  method: delete\n  operationId: deleteAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{id}/{field}\n  method: get\n  operationId: getActionField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/board\n  method: get\n  operationId: getActionBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/card\n  method: get\n  operationId: getActionCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/list\n  method: get\n  operationId: getActionList\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/member\n  method: get\n  operationId: getActionMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/memberCreator\n  method: get\n  operationId: getActionMemberCreator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/organization\n  method: get\n  operationId: getActionOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}/reactions\n  method: get\n  operationId: getActionReactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /actions/{id}/reactions\n  method: post\n  operationId: createActionReaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{id}/text\n  method: put\n  operationId: put-actions-id-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{idAction}/reactions\n  method: get\n  operationId: get-actions-idaction-reactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{idAction}/reactions\n  method: post\n  operationId: post-actions-idaction-reactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{idAction}/reactions/{id}\n  method: get\n  operationId: get-actions-idaction-reactions-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{idAction}/reactions/{id}\n  method: delete\n  operationId: delete-actions-idaction-reactions-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - read:board:trello\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{idAction}/reactionsSummary\n  method: get\n  operationId: get-actions-idaction-reactionsummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{key}/compliance\n  method: get\n  operationId: applications-key-compliance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch\n  method: get\n  operationId: get-batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards\n  method:\
  \ post\n  operationId: createBoard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}\n  method: get\n  operationId: getBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}\n  method: put\n  operationId: updateBoard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}\n  method: delete\n  operationId: deleteBoard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/actions\n  method: get\n  operationId: getBoardActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/cards\n  method: get\n  operationId: getBoardCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/cards/{filter}\n  method: get\n  operationId: getBoardCardsFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/checklists\n  method: get\n  operationId: getBoardChecklists\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/labels\n  method: get\n  operationId: getBoardLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/labels\n  method: post\n  operationId: createBoardLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/lists\n  method: get\n  operationId: getBoardLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/lists\n  method: post\n  operationId: createBoardList\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/members\n  method: get\n  operationId: getBoardMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/members\n  method: put\n  operationId: inviteBoardMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/members/{idMember}\n  method: put\n  operationId: updateBoardMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/members/{idMember}\n  method: delete\n  operationId: removeBoardMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/memberships\n  method: get\n  operationId: getBoardMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/{field}\n  method: get\n  operationId: get-boards-id-field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    -\
  \ read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{boardId}/actions\n  method: get\n  operationId: get-boards-id-actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{boardId}/boardStars\n  method: get\n  operationId: get-boards-id-boardstars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/customFields\n  method: get\n  operationId: get-boards-id-customfields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/lists/{filter}\n  method: get\n  operationId: get-boards-id-lists-filter\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/memberships/{idMembership}\n  method: put\n  operationId: put-boards-id-memberships-idmembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:board:membership:trello\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/myPrefs/emailPosition\n  method: put\n  operationId: put-boards-id-myprefs-emailposition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/myPrefs/idEmailList\n  method: put\n  operationId: put-boards-id-myprefs-idemaillist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/myPrefs/showSidebar\n  method: put\n  operationId: put-boards-id-myPrefs-showsidebar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/myPrefs/showSidebarActivity\n  method: put\n\
  \  operationId: put-boards-id-myPrefs-showsidebaractivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/myPrefs/showSidebarBoardActions\n  method: put\n  operationId: put-boards-id-myPrefs-showsidebarboardactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/myPrefs/showSidebarMembers\n  method: put\n  operationId: put-boards-id-myPrefs-showsidebarmembers\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - read:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/\n  method: post\n  operationId: post-boards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/calendarKey/generate\n  method: post\n  operationId: post-boards-id-calendarkey-generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/emailKey/generate\n  method: post\n  operationId: post-boards-id-emailkey-generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/idTags\n  method: post\n  operationId: post-boards-id-idtags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/markAsViewed\n  method: post\n  operationId: post-boards-id-markedasviewed\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/boardPlugins\n  method: get\n  operationId: get-boards-id-boardplugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/boardPlugins\n  method: post\n  operationId: post-boards-id-boardplugins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/boardPlugins/{idPlugin}\n\
  \  method: delete\n  operationId: delete-boards-id-boardplugins\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /boards/{id}/plugins\n  method: get\n  operationId: get-board-id-plugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/exports\n  method: post\n  operationId: post-boards-id-exports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/exports/{idExport}\n  method: get\n  operationId: get-boards-id-exports-idexport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - write:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/exports/{idExport}\n  method: delete\n  operationId: delete-boards-id-exports-idexport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boards/{id}/exports/{idExport}/download\n  method: get\n  operationId: get-boards-id-exports-idexport-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - write:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boards/{id}/exports/mostRecent\n  method: get\n  operationId: get-boards-id-exports-mostrecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - write:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}\n  method: put\n  operationId: updateCard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}\n  method: delete\n  operationId: deleteCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/actions\n  method: get\n  operationId: getCardActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/actions/comments\n  method: post\n  operationId: createCardComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/attachments\n  method: get\n  operationId: getCardAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/attachments\n  method: post\n  operationId: createCardAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/checklists\n  method: get\n  operationId: getCardChecklists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /cards/{id}/checklists\n  method: post\n  operationId: createCardChecklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/labels\n  method: post\n  operationId: addCardLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/labels/{idLabel}\n  method: delete\n  operationId: removeCardLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/members\n  method: post\n  operationId: addCardMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/members\n  method: get\n  operationId: get-cards-id-members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/members/{idMember}\n  method: delete\n  operationId: removeCardMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/stickers\n  method: get\n  operationId: getCardStickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/stickers\n  method: post\n  operationId: addCardSticker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/{field}\n  method: get\n  operationId: get-cards-id-field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/attachments/{idAttachment}\n  method: get\n  operationId: get-cards-id-attachments-idattachment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/attachments/{idAttachment}\n  method: delete\n  operationId: deleted-cards-id-attachments-idattachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/board\n  method: get\n  operationId: get-cards-id-board\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/checkItemStates\n  method: get\n  operationId: get-cards-id-checkitemstates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/checkItem/{idCheckItem}\n  method: get\n  operationId: get-cards-id-checkitem-idcheckitem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/checkItem/{idCheckItem}\n  method: put\n  operationId: put-cards-id-checkitem-idcheckitem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/checkItem/{idCheckItem}\n  method: delete\n  operationId: delete-cards-id-checkitem-idcheckitem\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/list\n  method: get\n  operationId: get-cards-id-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/membersVoted\n  method: get\n  operationId: get-cards-id-membersvoted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/membersVoted\n  method: post\n  operationId: cardsidmembersvoted-1\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/pluginData\n  method: get\n  operationId: get-cards-id-plugindata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/stickers/{idSticker}\n  method: get\n  operationId: get-cards-id-stickers-idsticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/stickers/{idSticker}\n  method: delete\n  operationId: delete-cards-id-stickers-idsticker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/stickers/{idSticker}\n  method: put\n  operationId: put-cards-id-stickers-idsticker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/actions/{idAction}/comments\n  method: put\n  operationId: put-cards-id-actions-idaction-comments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:board:trello\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/actions/{idAction}/comments\n  method: delete\n  operationId: delete-cards-id-actions-id-comments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{idCard}/customField/{idCustomField}/item\n  method: put\n  operationId: put-cards-idcard-customfield-idcustomfield-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /cards/{idCard}/customFields\n  method: put\n  operationId: put-cards-idcard-customfields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}/customFieldItems\n  method: get\n  operationId: get-cards-id-customfielditems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:board:trello\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}/idLabels\n  method: post\n  operationId: post-cards-id-idlabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:board:trello\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (86 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/agentic-access/trello-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/agentic-access/trello-agentic-access.yml
summary_line: 277 operations · 142 acting · 1 human-in-the-loop
tags:
- Project Management
- Kanban
- Task Management
- Collaboration
- Productivity
- Workflows
- Boards
- Atlassian
---
