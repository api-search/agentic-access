---
acting_count: 84
action_class_counts:
  acting: 84
  connected: 53
api_specs:
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Members API
  slug: mighty-networks-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Spaces API
  slug: mighty-networks-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Posts API
  slug: mighty-networks-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Comments and Reactions API
  slug: mighty-networks-comments-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Events and RSVPs API
  slug: mighty-networks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Courses API
  slug: mighty-networks-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Plans and Subscriptions API
  slug: mighty-networks-plans-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Invites API
  slug: mighty-networks-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Badges and Tags API
  slug: mighty-networks-badges-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Custom Fields API
  slug: mighty-networks-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Polls and Questions API
  slug: mighty-networks-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Network and Collections API
  slug: mighty-networks-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
- filename: mighty-networks-admin-api-openapi.json
  format: json
  label: Mighty Networks Webhooks
  slug: mighty-networks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/openapi/mighty-networks-admin-api-openapi.json
consequence_counts:
  physical: 7
  read: 53
  safety-critical: 4
  write: 73
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Mighty Networks Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/v1/networks/{network_id}/members/{member_id}/password_resets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/v1/networks/{network_id}/plans/{id}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/v1/networks/{network_id}/purchases/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /admin/v1/networks/{network_id}/collections/{id}/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/v1/networks/{network_id}/invites
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /admin/v1/networks/{network_id}/members/{id}/network_membership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /admin/v1/networks/{network_id}/plans/{plan_id}/members/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /admin/v1/networks/{network_id}/subscriptions/{id}
operation_count: 137
overview: 'Mighty Networks exposes 137 API operations that an AI agent could call, of which 84 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 53 read, 73 write, 7 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mighty Networks
provider_slug: mighty-networks
slug: mighty-networks-agentic-access
source_filename: mighty-networks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mighty-networks-admin-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 137\n  by_action_class:\n    connected: 53\n    acting: 84\n  by_consequence:\n    read: 53\n    write: 73\n    physical: 7\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members\n  method: get\n  operationId: list_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members\n  method: post\n  operationId: create_members\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members/{user_id}/\n  method: get\n  operationId: show_member\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members/{user_id}/\n  method: patch\n  operationId: update_members\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members/{user_id}/\n  method: put\n\
  \  operationId: replace_members\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members/{user_id}/\n  method: delete\n  operationId: delete_members\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/members/{user_id}/ban\n  method: post\n  operationId: create_members\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/courseworks\n  method: get\n  operationId: list_courseworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/courseworks\n  method: post\n  operationId: create_courseworks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/courseworks/{id}/\n  method: get\n  operationId: show_coursework\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/courseworks/{id}/\n  method: patch\n  operationId: update_courseworks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/courseworks/{id}/\n  method: put\n  operationId: replace_courseworks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{space_id}/courseworks/{id}/\n  method: delete\n  operationId: delete_courseworks\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/reactions\n  method: get\n  operationId: list_reactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/reactions\n  method: post\n  operationId: create_reactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/reactions\n  method: delete\n  operationId:\
  \ delete_reactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/mute\n  method: post\n  operationId: create_mute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/mute\n  method: delete\n  operationId: delete_mute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/comments\n  method: get\n  operationId: list_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/comments\n  method: post\n  operationId: create_comments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/comments/{id}/\n  method: get\n  operationId: show_comment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/posts/{post_id}/comments/{id}/\n\
  \  method: delete\n  operationId: delete_comments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/members\n  method: get\n  operationId: list_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/members\n  method: post\n  operationId: create_members\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/members/{member_id}/\n\
  \  method: get\n  operationId: show_member\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites\n  method: get\n  operationId: list_invites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites\n  method: post\n  operationId: create_invites\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/\n  method: get\n  operationId: show_invite\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/\n  method: patch\n  operationId: update_invites\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/\n  method: put\n  operationId: replace_invites\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /admin/v1/networks/{network_id}/plans/{plan_id}/invites/{id}/\n  method: delete\n  operationId: delete_invites\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/v1/networks/{network_id}/members/{member_id}/tags\n  method: get\n  operationId: list_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{member_id}/tags\n  method: post\n  operationId: create_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/members/{member_id}/tags/{tag_id}/\n  method: get\n  operationId: show_tag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{member_id}/tags/{tag_id}/\n  method: delete\n  operationId: delete_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/members/{member_id}/spaces\n  method: get\n  operationId: list_spaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{member_id}/plans\n\
  \  method: get\n  operationId: list_plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{member_id}/password_resets\n  method: post\n  operationId: create_password_resets\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/v1/networks/{network_id}/members/{member_id}/badges\n  method: get\n  operationId: list_badges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{member_id}/badges\n  method: post\n  operationId: create_badges\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/members/{member_id}/badges/{badge_id}/\n  method: get\n  operationId: show_badge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{member_id}/badges/{badge_id}/\n  method: delete\n  operationId: delete_badges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/events/{event_id}/rsvps\n\
  \  method: get\n  operationId: list_rsvps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/events/{event_id}/rsvps\n  method: post\n  operationId: create_rsvps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/events/{event_id}/rsvps/{id}/\n  method: get\n  operationId: show_rsvp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/events/{event_id}/rsvps/{id}/\n  method: patch\n  operationId: update_rsvps\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/events/{event_id}/rsvps/{id}/\n  method: put\n  operationId: replace_rsvps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/events/{event_id}/rsvps/{id}/\n  method: delete\n  operationId: delete_rsvps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/options\n  method: get\n  operationId: list_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/options\n  method: post\n  operationId: create_options\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/options/{id}/\n  method: get\n  operationId: show_option\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/options/{id}/\n\
  \  method: patch\n  operationId: update_options\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/options/{id}/\n  method: put\n  operationId: replace_options\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/options/{id}/\n  method: delete\n  operationId: delete_options\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/members/{member_id}/answers\n  method: get\n  operationId: list_answers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/members/{member_id}/answers\n  method: post\n  operationId: create_answers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/members/{member_id}/answers\n  method: delete\n  operationId:\
  \ delete_answers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/custom_fields/{custom_field_id}/members/{member_id}/answers/{id}/\n  method: get\n  operationId: show_answer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/comments/{comment_id}/reactions\n  method: get\n  operationId: list_reactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/comments/{comment_id}/reactions\n  method: post\n  operationId: create_reactions\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/comments/{comment_id}/reactions\n  method: delete\n  operationId: delete_reactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/tags\n  method: get\n  operationId: list_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/tags\n  method: post\n  operationId: create_tags\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/tags/{id}/\n  method: get\n  operationId: show_tag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/tags/{id}/\n  method: patch\n  operationId: update_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/tags/{id}/\n  method: put\n  operationId: replace_tags\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/tags/{id}/\n  method: delete\n  operationId: delete_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/subscriptions\n  method: get\n  operationId: list_subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/subscriptions/{id}\n  method: get\n  operationId: show_subscription\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/subscriptions/{id}\n  method: delete\n  operationId: delete_subscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces\n  method: get\n  operationId: list_spaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/spaces\n  method: post\n  operationId: create_spaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{id}\n  method: get\n  operationId: show_space\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/spaces/{id}\n  method: patch\n  operationId: update_spaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{id}\n  method: put\n  operationId: replace_spaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/spaces/{id}\n  method: delete\n  operationId: delete_spaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/purchases\n  method: get\n  operationId: list_purchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/purchases/{id}/\n  method: get\n  operationId: show_purchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/purchases/{id}/\n  method: delete\n  operationId: delete_purchases\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts\n  method: get\n  operationId: list_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/posts\n  method: post\n  operationId: create_posts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{id}/\n  method: get\n  operationId: show_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/posts/{id}/\n  method: patch\n  operationId: update_posts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{id}/\n  method: put\n  operationId: replace_posts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/posts/{id}/\n  method: delete\n  operationId: delete_posts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/polls\n  method: get\n  operationId: list_polls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/polls\n  method: post\n  operationId: create_polls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/polls/{id}/\n  method: get\n  operationId: show_poll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/polls/{id}/\n  method: patch\n  operationId: update_polls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/polls/{id}/\n  method: put\n  operationId: replace_polls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /admin/v1/networks/{network_id}/polls/{id}/\n  method: delete\n  operationId: delete_polls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/plans\n  method: get\n  operationId: list_plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/plans/{id}/\n  method: get\n  operationId: show_plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/plans/{id}/\n  method: delete\n  operationId: delete_plans\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/v1/networks/{network_id}/plans/{plan_id}/members/{id}/\n  method: delete\n  operationId: delete_plans\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/\n  method: get\n  operationId: show_network\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members\n\
  \  method: get\n  operationId: list_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members\n  method: post\n  operationId: create_members\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/v1/networks/{network_id}/members/{id}/\n  method: get\n  operationId: show_member\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/networks/{network_id}/members/{id}/\n  method: pat\n\n# --- truncated at 32 KB (44 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/agentic-access/mighty-networks-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mighty-networks/refs/heads/main/agentic-access/mighty-networks-agentic-access.yml
summary_line: 137 operations · 84 acting · 4 human-in-the-loop
tags:
- Community
- Courses
- Membership
- Creator Economy
- Events
- Subscriptions
---
