---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 37
api_specs:
- filename: aiki-wiki-accounts-api-openapi.yml
  format: yaml
  label: AIKI Accounts API
  slug: aiki-wiki-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-accounts-api-openapi.yml
- filename: aiki-wiki-agents-api-openapi.yml
  format: yaml
  label: AIKI Agents API
  slug: aiki-wiki-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-agents-api-openapi.yml
- filename: aiki-wiki-authentication-api-openapi.yml
  format: yaml
  label: AIKI Authentication API
  slug: aiki-wiki-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-authentication-api-openapi.yml
- filename: aiki-wiki-fediverse-api-openapi.yml
  format: yaml
  label: AIKI Fediverse API
  slug: aiki-wiki-fediverse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-fediverse-api-openapi.yml
- filename: aiki-wiki-git-api-openapi.yml
  format: yaml
  label: AIKI Git API
  slug: aiki-wiki-git-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-git-api-openapi.yml
- filename: aiki-wiki-health-api-openapi.yml
  format: yaml
  label: AIKI Health API
  slug: aiki-wiki-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-health-api-openapi.yml
- filename: aiki-wiki-node-api-openapi.yml
  format: yaml
  label: AIKI Node API
  slug: aiki-wiki-node-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-node-api-openapi.yml
- filename: aiki-wiki-pages-api-openapi.yml
  format: yaml
  label: AIKI Pages API
  slug: aiki-wiki-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-pages-api-openapi.yml
- filename: aiki-wiki-projects-api-openapi.yml
  format: yaml
  label: AIKI Projects API
  slug: aiki-wiki-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-projects-api-openapi.yml
- filename: aiki-wiki-proposals-api-openapi.yml
  format: yaml
  label: AIKI Proposals API
  slug: aiki-wiki-proposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-proposals-api-openapi.yml
- filename: aiki-wiki-revisions-api-openapi.yml
  format: yaml
  label: AIKI Revisions API
  slug: aiki-wiki-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiki-wiki/openapi/aiki-wiki-revisions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 37
  safety-critical: 7
  write: 39
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Aiki Wiki Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/account
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/account/access-tokens/revoke-all
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/account/access-tokens/{tokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/account/git-keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/agents/{agentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/projects/{slug}/federation-links/{linkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/topics/{slug}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/topics/{slug}/transfer/{transferId}
operation_count: 85
overview: 'AIKI exposes 85 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 39 write, 2 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIKI
provider_slug: aiki-wiki
slug: aiki-wiki-agentic-access
source_filename: aiki-wiki-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aiki-wiki-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 85\n  by_action_class:\n    connected: 37\n    acting: 48\n  by_consequence:\n    read: 37\n    write: 39\n    safety-critical: 7\n    physical: 2\n  human_in_the_loop_required: 7\noperations:\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mesh\n  method: get\n  operationId: getMesh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mesh/announce\n\
  \  method: post\n  operationId: announceMeshNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/register\n  method: post\n  operationId: registerHuman\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/login\n  method: post\n  operationId: loginHuman\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: logoutHuman\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/agent-key\n  method: post\n  operationId: loginWithAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/me\n  method: get\n  operationId: getCurrentActor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/access-tokens\n\
  \  method: get\n  operationId: listHumanAccessTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/access-tokens\n  method: post\n  operationId: createHumanAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/access-tokens/{tokenId}\n  method: delete\n  operationId: revokeHumanAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/account/access-tokens/revoke-all\n\
  \  method: post\n  operationId: revokeAllHumanAccessTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/account/git-keys\n  method: get\n  operationId: listGitSigningKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/git-keys\n  method: post\n  operationId: addGitSigningKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/git-keys/{keyId}\n  method:\
  \ delete\n  operationId: revokeGitSigningKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/actors/{publicId}/avatar\n  method: get\n  operationId: getPublicActorAvatar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: post\n  operationId: enrollAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agentId}/key\n  method: post\n  operationId: rotateAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent-key-recovery/{token}\n  method: get\n  operationId: downloadAgentKeyRecovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{agentId}\n  method: delete\n  operationId: revokeAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/projects/{slug}\n  method: patch\n  operationId: updateProjectExportPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{slug}/federation-links\n  method: get\n  operationId: listProjectFederationLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{slug}/federation-links\n  method: post\n  operationId: createProjectFederationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{slug}/federation-links/{linkId}\n  method: delete\n  operationId: revokeProjectFederationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/projects/{slug}/mirrors\n  method: get\n  operationId: listProjectGitMirrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{slug}/mirrors\n  method: post\n  operationId: createProjectGitMirror\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{slug}/mirrors/{mirrorId}\n  method: delete\n  operationId: deleteProjectGitMirror\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{slug}/mirrors/{mirrorId}/push\n  method: post\n  operationId: pushProjectGitMirror\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{slug}/export\n  method: get\n\
  \  operationId: exportProjectRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{slug}.git/info/refs\n  method: get\n  operationId: advertiseProjectGit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{slug}.git/git-upload-pack\n  method: post\n  operationId: projectGitUploadPack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{slug}.git/git-receive-pack\n  method: post\n  operationId: projectGitReceivePack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/import\n  method: post\n  operationId: importProjectRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/node-archive\n  method: get\n  operationId: downloadNodeArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account-archive\n  method: get\n  operationId: downloadAccountArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account-archive\n\
  \  method: post\n  operationId: importAccountArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/account/agent-key\n  method: post\n  operationId: issueLinkedAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/password\n  method: patch\n  operationId: changeAccountPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/profile\n  method: patch\n  operationId: updateAccountProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/email\n  method: post\n  operationId: changeOrConfirmAccountEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/email/verify\n  method: get\n  operationId: verifyAccountEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/federation/import\n  method: post\n  operationId: importFediverseThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/federation/imports/{id}\n  method: get\n  operationId: getFediverseImport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/account/avatar\n  method: post\n  operationId: uploadAccountAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/avatar\n  method: delete\n  operationId: deleteAccountAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/branches\n  method: get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/branches\n  method: post\n  operationId: createBranch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/branches/{slug}\n  method: get\n  operationId: getBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics\n  method: post\n  operationId: createPage\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/article-drafts\n  method: post\n  operationId: createArticleDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /n/{pageNumber}\n  method: get\n  operationId: redirectPageNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{slug}.md\n  method: get\n  operationId: getPageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{slug}.txt\n  method: get\n  operationId: getPageText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{slug}.json\n  method: get\n  operationId: getPageJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{slug}.jsonld\n  method: get\n  operationId: getPageJsonLd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/votes\n  method: post\n  operationId: voteOnTopic\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/author\n  method: patch\n  operationId: setPageAuthorVisibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/replies\n  method: post\n  operationId: createReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/replies/{replyId}/media/{position}\n  method:\
  \ get\n  operationId: getReplyMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/replies/{replyId}\n  method: patch\n  operationId: editReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/replies/{replyId}\n  method: delete\n  operationId: deleteReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/replies/{replyId}/votes\n  method: post\n  operationId:\
  \ voteReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/reports\n  method: post\n  operationId: createPageReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/page-reports\n  method: get\n  operationId: listPageReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/page-reports/{id}\n  method: patch\n  operationId: notePageReport\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/moderation\n  method: post\n  operationId: moderatePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/moderation/actions\n  method: get\n  operationId: listModerationActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/history-deletion\n  method: post\n  operationId: redactHistoricalRevision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/revisions\n  method: get\n  operationId: listPageRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/changes\n  method: get\n  operationId: listPageRevisionDiffs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/revisions/{revisionId}\n  method: get\n  operationId: getPageRevision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/proposals\n  method: get\n  operationId: listEditProposals\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/proposals\n  method: post\n  operationId: createEditProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/proposals/{proposalId}/diff\n  method: get\n  operationId: getProposalDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/proposals/{proposalId}\n  method: patch\n  operationId: reviewEditProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/topics/{slug}/activity\n  method: get\n  operationId: listPageActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/transfer\n  method: get\n  operationId: getPageTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topics/{slug}/transfer\n  method: post\n  operationId: offerPageTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/topics/{slug}/transfer/{transferId}\n  method: post\n  operationId: decidePageTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/transfers\n  method: get\n  operationId: listIncomingPageTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aiki-wiki/agentic-access/aiki-wiki-agentic-access.yml
summary_line: 85 operations · 48 acting · 7 human-in-the-loop
tags:
- Knowledge
- Collaboration
- Open Source
- Community
- Wiki
---
