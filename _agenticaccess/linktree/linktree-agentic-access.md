---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Linktree Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Linktree exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Linktree
provider_slug: linktree
slug: linktree-agentic-access
source_filename: linktree-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "# Agentic access contract — sourced from Linktree's OWN published per-tool access,\n# approval, and identity classifications (not heuristically inferred).\ngenerated: '2026-07-19'\nmethod: searched\nsource: https://mcp.linktr.ee/.well-known/mcp/tools.json\nmodel: x-agentic-access\nsummary:\n  operation_count: 30\n  by_access:\n    read: 19\n    write: 9\n    destructive: 2\n  approval_required: 11\n  approval_hint_header: x-linktree-require-approval\n  auth: oauth2 per-tool scope (mcp:<tool>)\n  audience: null\noperations:\n  - operation: list_accessible_profiles\n    action_class: read\n    consequence: read\n    scope: mcp:list_accessible_profiles\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: set_active_profile\n    action_class: read\n    consequence: read\n    scope: mcp:set_active_profile\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: get_account\n    action_class: read\n    consequence:\
  \ read\n    scope: mcp:get_account\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: update_account_profile\n    action_class: acting\n    consequence: write\n    scope: mcp:update_account_profile\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: get_suggested_bio\n    action_class: read\n    consequence: read\n    scope: mcp:get_suggested_bio\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_account_analytics\n    action_class: read\n    consequence: read\n    scope: mcp:get_account_analytics\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_analytics_lifetime_totals\n    action_class: read\n    consequence: read\n    scope: mcp:get_analytics_lifetime_totals\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_top_links\n\
  \    action_class: read\n    consequence: read\n    scope: mcp:get_top_links\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_profile_views\n    action_class: read\n    consequence: read\n    scope: mcp:get_profile_views\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_social_integrations\n    action_class: read\n    consequence: read\n    scope: mcp:get_social_integrations\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_appearance\n    action_class: read\n    consequence: read\n    scope: mcp:get_appearance\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: update_appearance\n    action_class: acting\n    consequence: write\n    scope: mcp:update_appearance\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: get_knowledge_base\n\
  \    action_class: read\n    consequence: read\n    scope: mcp:get_knowledge_base\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_workspaces_for_user\n    action_class: read\n    consequence: read\n    scope: mcp:get_workspaces_for_user\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: get_workspace\n    action_class: read\n    consequence: read\n    scope: mcp:get_workspace\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: get_workspace_profiles\n    action_class: read\n    consequence: read\n    scope: mcp:get_workspace_profiles\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: get_workspace_profiles_analytics\n    action_class: read\n    consequence: read\n    scope: mcp:get_workspace_profiles_analytics\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: get_workspace_members\n\
  \    action_class: read\n    consequence: read\n    scope: mcp:get_workspace_members\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user\"\n  - operation: get_links\n    action_class: read\n    consequence: read\n    scope: mcp:get_links\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: add_link\n    action_class: acting\n    consequence: write\n    scope: mcp:add_link\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: create_collection\n    action_class: acting\n    consequence: write\n    scope: mcp:create_collection\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: add_links_to_collection\n    action_class: acting\n    consequence: write\n    scope: mcp:add_links_to_collection\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: update_link\n    action_class:\
  \ acting\n    consequence: write\n    scope: mcp:update_link\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: reorder_link\n    action_class: acting\n    consequence: write\n    scope: mcp:reorder_link\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: delete_link\n    action_class: acting\n    consequence: destructive\n    scope: mcp:delete_link\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: get_link_analytics\n    action_class: read\n    consequence: read\n    scope: mcp:get_link_analytics\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: get_social_links\n    action_class: read\n    consequence: read\n    scope: mcp:get_social_links\n    human_in_the_loop: none\n    audit: optional\n    identity: \"user_or_account\"\n  - operation: upsert_social_link\n    action_class:\
  \ acting\n    consequence: write\n    scope: mcp:upsert_social_link\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: reorder_social_links\n    action_class: acting\n    consequence: write\n    scope: mcp:reorder_social_links\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n  - operation: delete_social_link\n    action_class: acting\n    consequence: destructive\n    scope: mcp:delete_social_link\n    human_in_the_loop: required\n    audit: required\n    identity: \"user_or_account\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linktree/refs/heads/main/agentic-access/linktree-agentic-access.yml
summary_line: 30 operations
tags:
- Company
- Media
- Link in Bio
- Creator Economy
- Social Media
- Marketing
- Analytics
- MCP
- Agents
---
