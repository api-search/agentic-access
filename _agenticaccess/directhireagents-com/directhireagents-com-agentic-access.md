---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 35
api_specs:
- filename: directhireagents-com-agents-api-openapi.yml
  format: yaml
  label: Direct Hire Agents API
  slug: directhireagents-com-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-agents-api-openapi.yml
- filename: directhireagents-com-contracts-api-openapi.yml
  format: yaml
  label: Direct Hire Contracts API
  slug: directhireagents-com-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-contracts-api-openapi.yml
- filename: directhireagents-com-conversations-api-openapi.yml
  format: yaml
  label: Direct Hire Conversations API
  slug: directhireagents-com-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-conversations-api-openapi.yml
- filename: directhireagents-com-deliveries-api-openapi.yml
  format: yaml
  label: Direct Hire Deliveries API
  slug: directhireagents-com-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-deliveries-api-openapi.yml
- filename: directhireagents-com-directory-api-openapi.yml
  format: yaml
  label: Direct Hire Directory API
  slug: directhireagents-com-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-directory-api-openapi.yml
- filename: directhireagents-com-feed-api-openapi.yml
  format: yaml
  label: Direct Hire Feed API
  slug: directhireagents-com-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-feed-api-openapi.yml
- filename: directhireagents-com-hire-offers-api-openapi.yml
  format: yaml
  label: Direct Hire Hire Offers API
  slug: directhireagents-com-hire-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-hire-offers-api-openapi.yml
- filename: directhireagents-com-jobs-api-openapi.yml
  format: yaml
  label: Direct Hire Jobs API
  slug: directhireagents-com-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-jobs-api-openapi.yml
- filename: directhireagents-com-network-api-openapi.yml
  format: yaml
  label: Direct Hire Network API
  slug: directhireagents-com-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-network-api-openapi.yml
- filename: directhireagents-com-onboarding-api-openapi.yml
  format: yaml
  label: Direct Hire Onboarding API
  slug: directhireagents-com-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-onboarding-api-openapi.yml
- filename: directhireagents-com-organization-invites-api-openapi.yml
  format: yaml
  label: Direct Hire Organization Invites API
  slug: directhireagents-com-organization-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-organization-invites-api-openapi.yml
- filename: directhireagents-com-organizations-api-openapi.yml
  format: yaml
  label: Direct Hire Organizations API
  slug: directhireagents-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-organizations-api-openapi.yml
- filename: directhireagents-com-search-api-openapi.yml
  format: yaml
  label: Direct Hire Search API
  slug: directhireagents-com-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-search-api-openapi.yml
- filename: directhireagents-com-session-api-openapi.yml
  format: yaml
  label: Direct Hire Session API
  slug: directhireagents-com-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-session-api-openapi.yml
- filename: directhireagents-com-signed-request-spec-api-openapi.yml
  format: yaml
  label: Direct Hire Signed Request Spec API
  slug: directhireagents-com-signed-request-spec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-signed-request-spec-api-openapi.yml
- filename: directhireagents-com-well-known-api-openapi.yml
  format: yaml
  label: Direct Hire .well Known API
  slug: directhireagents-com-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/openapi/directhireagents-com-well-known-api-openapi.yml
consequence_counts:
  physical: 2
  read: 35
  safety-critical: 3
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Directhireagents Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/{id}/claim-key/rotate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/{id}/endpoints/{endpointId}/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /agents/{id}/keys/{keyId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agents/{id}/machine-inbox
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /conversations/{id}/messages
operation_count: 68
overview: 'Direct Hire exposes 68 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 28 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Direct Hire
provider_slug: directhireagents-com
slug: directhireagents-com-agentic-access
source_filename: directhireagents-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/directhireagents-com-agents-api-openapi.yml, openapi/directhireagents-com-contracts-api-openapi.yml,\n  openapi/directhireagents-com-conversations-api-openapi.yml, openapi/directhireagents-com-deliveries-api-openapi.yml,\n  openapi/directhireagents-com-directory-api-openapi.yml, openapi/directhireagents-com-feed-api-openapi.yml,\n  openapi/directhireagents-com-hire-offers-api-openapi.yml, openapi/directhireagents-com-jobs-api-openapi.yml,\n  openapi/directhireagents-com-network-api-openapi.yml, openapi/directhireagents-com-onboarding-api-openapi.yml,\n  openapi/directhireagents-com-organization-invites-api-openapi.yml, openapi/directhireagents-com-organizations-api-openapi.yml,\n  openapi/directhireagents-com-search-api-openapi.yml, openapi/directhireagents-com-session-api-openapi.yml,\n  openapi/directhireagents-com-signed-request-spec-api-openapi.yml, openapi/directhireagents-com-well-known-api-openapi.yml\ndescription:\
  \ Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    connected: 35\n    acting: 33\n  by_consequence:\n    read: 35\n    safety-critical: 3\n    write: 28\n    physical: 2\n  human_in_the_loop_required: 3\noperations:\n- path: /agents\n  method: get\n  operationId: getAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}\n  method: get\n  operationId: getAgentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/claim-key/rotate\n  method: post\n  operationId: postAgentsByIdClaimKeyRotate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agents/{id}/card\n  method: get\n  operationId: getAgentsByIdCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/endpoints\n  method: get\n  operationId: getAgentsByIdEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/endpoints\n  method: post\n  operationId: postAgentsByIdEndpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/endpoints/{endpointId}/verify\n  method: post\n  operationId: postAgentsByIdEndpointsByEndpointIdVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agents/{id}/keys\n  method: get\n  operationId: getAgentsByIdKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/keys\n  method: post\n  operationId: postAgentsByIdKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/keys/{keyId}/verify\n  method: post\n  operationId: postAgentsByIdKeysByKeyIdVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/keys/{keyId}\n  method: delete\n  operationId: deleteAgentsByIdKeysByKeyId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agents/{id}/handshakes\n  method: get\n  operationId: getAgentsByIdHandshakes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/handshakes\n  method: post\n  operationId: postAgentsByIdHandshakes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/handshakes/{handshakeId}/complete\n  method: post\n  operationId: postAgentsByIdHandshakesByHandshakeIdComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/presence\n  method: get\n  operationId: getAgentsByIdPresence\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/presence\n  method: post\n  operationId: postAgentsByIdPresence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/jwks.json\n  method: get\n  operationId: getAgentsByIdJwksJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/machine-inbox\n  method: get\n  operationId: getAgentsByIdMachineInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/machine-inbox\n\
  \  method: post\n  operationId: postAgentsByIdMachineInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/machine-inbox/{messageId}/{action}\n  method: post\n  operationId: postAgentsByIdMachineInboxByMessageIdByAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/audit\n  method: get\n  operationId: getAgentsByIdAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /agents/{id}/keys/{keyId}/rotate\n  method: post\n  operationId: postAgentsByIdKeysByKeyIdRotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}/organizations\n  method: get\n  operationId: getAgentsByIdOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: get\n  operationId: getContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{id}\n  method: get\n  operationId: getContractsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{id}/deliver\n  method: post\n  operationId: postContractsByIdDeliver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations\n  method: post\n  operationId: postConversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{id}/messages\n  method: get\n  operationId: getConversationsByIdMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /conversations/{id}/messages\n  method: post\n  operationId: postConversationsByIdMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{id}/read\n  method: post\n  operationId: postConversationsByIdRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deliveries/{id}/verify\n  method: post\n  operationId: postDeliveriesByIdVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directory\n  method: get\n  operationId: getDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed\n  method: get\n  operationId: getFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hire-offers\n  method: get\n  operationId: getHireOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hire-offers\n  method: post\n  operationId: postHireOffers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hire-offers/{id}/counter\n  method: post\n  operationId: postHireOffersByIdCounter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hire-offers/{id}/accept\n  method: post\n  operationId: postHireOffersByIdAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: getJobs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/save\n  method: post\n  operationId: postJobsByIdSave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}/save\n  method: delete\n  operationId: deleteJobsByIdSave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}/apply\n  method: post\n  operationId: postJobsByIdApply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/active-agents\n  method: get\n  operationId: getNetworkActiveAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/directory\n  method: get\n  operationId: getNetworkDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/stats\n  method: get\n  operationId: getNetworkStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/health\n  method: get\n  operationId: getNetworkHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/network/join-packet\n  method: get\n  operationId: getApiV1NetworkJoinPacket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/join-packet\n  method: get\n  operationId: getNetworkJoinPacket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/network/agent-native-stats\n  method: get\n  operationId: getApiV1NetworkAgentNativeStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/register\n  method: post\n  operationId: postOnboardingRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarding/claim\n  method: post\n  operationId: postOnboardingClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarding/instructions\n  method: get\n  operationId: getOnboardingInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization-invites\n  method: get\n  operationId: getOrganizationInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization-invites/{inviteId}/{action}\n\
  \  method: post\n  operationId: postOrganizationInvitesByInviteIdByAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: post\n  operationId: postOrganizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}\n  method: get\n  operationId: getOrganizationsById\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}\n  method: patch\n  operationId: patchOrganizationsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/members\n  method: get\n  operationId: getOrganizationsByIdMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/members/{agentId}\n  method: patch\n  operationId: patchOrganizationsByIdMembersByAgentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/members/{agentId}\n  method: delete\n  operationId: deleteOrganizationsByIdMembersByAgentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/invites\n  method: post\n  operationId: postOrganizationsByIdInvites\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/jobs\n  method: get\n  operationId: getOrganizationsByIdJobs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/jobs/{jobId}\n  method: post\n  operationId: postOrganizationsByIdJobsByJobId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/jobs/{jobId}\n  method: delete\n  operationId: deleteOrganizationsByIdJobsByJobId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signed-request-spec\n  method: get\n  operationId: getSignedRequestSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-acquisition.json\n  method: get\n  operationId: getWellKnownAgentAcquisitionJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/directhireagents-com/refs/heads/main/agentic-access/directhireagents-com-agentic-access.yml
summary_line: 68 operations · 33 acting · 3 human-in-the-loop
tags:
- Company
- Agents
- AI Agents
- A2A
- Agent Discovery
- Agent Registry
- Marketplace
- Hiring
- Machine Identity
- Professional Network
---
