---
acting_count: 76
action_class_counts:
  acting: 76
  connected: 61
api_specs:
- filename: agentboxd-com-agent-network-api-openapi.yml
  format: yaml
  label: agentboxd-com Agent network API
  slug: agentboxd-com-agent-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-agent-network-api-openapi.yml
- filename: agentboxd-com-agent-self-signup-api-openapi.yml
  format: yaml
  label: agentboxd-com Agent self-signup API
  slug: agentboxd-com-agent-self-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-agent-self-signup-api-openapi.yml
- filename: agentboxd-com-contacts-api-openapi.yml
  format: yaml
  label: agentboxd-com Contacts API
  slug: agentboxd-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-contacts-api-openapi.yml
- filename: agentboxd-com-domains-api-openapi.yml
  format: yaml
  label: agentboxd-com Domains API
  slug: agentboxd-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-domains-api-openapi.yml
- filename: agentboxd-com-drafts-api-openapi.yml
  format: yaml
  label: agentboxd-com Drafts API
  slug: agentboxd-com-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-drafts-api-openapi.yml
- filename: agentboxd-com-events-api-openapi.yml
  format: yaml
  label: agentboxd-com Events API
  slug: agentboxd-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-events-api-openapi.yml
- filename: agentboxd-com-inboxes-api-openapi.yml
  format: yaml
  label: agentboxd-com Inboxes API
  slug: agentboxd-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-inboxes-api-openapi.yml
- filename: agentboxd-com-knowledge-api-openapi.yml
  format: yaml
  label: agentboxd-com Knowledge API
  slug: agentboxd-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-knowledge-api-openapi.yml
- filename: agentboxd-com-lists-api-openapi.yml
  format: yaml
  label: agentboxd-com Lists API
  slug: agentboxd-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-lists-api-openapi.yml
- filename: agentboxd-com-messages-api-openapi.yml
  format: yaml
  label: agentboxd-com Messages API
  slug: agentboxd-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-messages-api-openapi.yml
- filename: agentboxd-com-metrics-api-openapi.yml
  format: yaml
  label: agentboxd-com Metrics API
  slug: agentboxd-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-metrics-api-openapi.yml
- filename: agentboxd-com-other-api-openapi.yml
  format: yaml
  label: agentboxd-com Other API
  slug: agentboxd-com-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-other-api-openapi.yml
- filename: agentboxd-com-search-api-openapi.yml
  format: yaml
  label: agentboxd-com Search API
  slug: agentboxd-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-search-api-openapi.yml
- filename: agentboxd-com-shakehand-api-openapi.yml
  format: yaml
  label: agentboxd-com Shakehand API
  slug: agentboxd-com-shakehand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-shakehand-api-openapi.yml
- filename: agentboxd-com-threads-api-openapi.yml
  format: yaml
  label: agentboxd-com Threads API
  slug: agentboxd-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-threads-api-openapi.yml
- filename: agentboxd-com-trust-api-openapi.yml
  format: yaml
  label: agentboxd-com Trust API
  slug: agentboxd-com-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-trust-api-openapi.yml
- filename: agentboxd-com-webhooks-api-openapi.yml
  format: yaml
  label: agentboxd-com Webhooks API
  slug: agentboxd-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentboxd-com/openapi/agentboxd-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 8
  read: 61
  safety-critical: 4
  write: 64
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Agentboxd Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/emergency-stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/inboxes/{id}/agent/keys/{kid}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/inboxes/{id}/agent/restore
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/inboxes/{id}/agent/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/drafts/{draftId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/forwarding/{forwardId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/inboxes/{id}/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/deliveries/{deliveryId}/redeliver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/redeliver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/test
operation_count: 137
overview: 'agentboxd-com exposes 137 API operations that an AI agent could call, of which 76 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read, 64 write, 8 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agentboxd-com
provider_slug: agentboxd-com
slug: agentboxd-com-agentic-access
source_filename: agentboxd-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/agentboxd-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 137\n  by_action_class:\n    connected: 61\n    acting: 76\n  by_consequence:\n    read: 61\n    write: 64\n    safety-critical: 4\n    physical: 8\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/attachments/{id}\n  method: get\n  operationId: getAttachmentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /v1/contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/{id}\n  method: get\n  operationId: getContactsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/{id}\n  method: patch\n  operationId: patchContactsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/{id}\n  method: delete\n  operationId: deleteContactsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/by-address/{address}\n  method: get\n  operationId: getContactsByAddressByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/delete\n  method: post\n  operationId: postContactsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/domains\n  method: get\n  operationId: getContactsDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/deliverability\n  method: get\n  operationId: getDeliverability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/handle\n  method: get\n  operationId: getDirectoryHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/handle\n  method: put\n  operationId: putDirectoryHandle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/directory/handle\n  method: delete\n  operationId: deleteDirectoryHandle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/directory/reports\n  method: post\n  operationId: postDirectoryReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/directory/resolve\n  method: get\n  operationId: getDirectoryResolve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/search\n  method: get\n  operationId: getDirectorySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/verify\n\
  \  method: post\n  operationId: postDirectoryVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains\n  method: post\n  operationId: postDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains\n  method: get\n  operationId: getDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}\n  method: get\n  operationId: getDomainsById\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}\n  method: patch\n  operationId: patchDomainsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}\n  method: delete\n  operationId: deleteDomainsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/dkim/activate\n  method: post\n  operationId: postDomainsByIdDkimActivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/dkim/rotate\n  method: post\n  operationId: postDomainsByIdDkimRotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/verify\n  method: post\n  operationId: postDomainsByIdVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/zone-file\n  method: get\n  operationId: getDomainsByIdZoneFile\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drafts\n  method: get\n  operationId: getDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/emergency-stop\n  method: post\n  operationId: postEmergencyStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/escalation\n  method: get\n  operationId: getEscalation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/escalation\n  method: put\n\
  \  operationId: putEscalation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identities\n  method: post\n  operationId: postIdentities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identities\n  method: get\n  operationId: getIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/identities/{id}\n  method: get\n  operationId: getIdentitiesById\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/identities/{id}\n  method: patch\n  operationId: patchIdentitiesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identities/{id}\n  method: delete\n  operationId: deleteIdentitiesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identity/clients\n  method: get\n  operationId: getIdentityClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/identity/clients\n  method: post\n  operationId: postIdentityClients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identity/clients/{id}\n  method: get\n  operationId: getIdentityClientsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/identity/clients/{id}\n  method: patch\n  operationId: patchIdentityClientsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/identity/clients/{id}\n  method: delete\n  operationId: deleteIdentityClientsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identity/clients/{id}/secret\n  method: post\n  operationId: postIdentityClientsByIdSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes\n  method: post\n  operationId: postInboxes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes\n  method: get\n  operationId: getInboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}\n  method: get\n  operationId: getInboxesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}\n  method: patch\n  operationId: patchInboxesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}\n  method: delete\n  operationId: deleteInboxesById\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/agent\n  method: get\n  operationId: getInboxesByIdAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/agent\n  method: patch\n  operationId: patchInboxesByIdAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/agent\n  method: delete\n  operationId: deleteInboxesByIdAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/agent/keys\n  method: get\n  operationId: getInboxesByIdAgentKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/agent/keys\n  method: post\n  operationId: postInboxesByIdAgentKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/agent/keys/{kid}/retire\n  method: post\n  operationId: postInboxesByIdAgentKeysByKidRetire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/agent/keys/{kid}/revoke\n  method: post\n  operationId: postInboxesByIdAgentKeysByKidRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/inboxes/{id}/agent/oasf\n  method: get\n  operationId: getInboxesByIdAgentOasf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/agent/restore\n  method: post\n  operationId: postInboxesByIdAgentRestore\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/inboxes/{id}/agent/revoke\n  method: post\n  operationId: postInboxesByIdAgentRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/inboxes/{id}/drafts\n  method: post\n  operationId: postInboxesByIdDrafts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts\n  method: get\n  operationId: getInboxesByIdDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/drafts/{draftId}\n  method: get\n  operationId: getInboxesByIdDraftsByDraftId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/drafts/{draftId}\n  method: patch\n  operationId: patchInboxesByIdDraftsByDraftId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts/{draftId}\n  method: delete\n  operationId: deleteInboxesByIdDraftsByDraftId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts/{draftId}/cancel\n  method: post\n  operationId: postInboxesByIdDraftsByDraftIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts/{draftId}/schedule\n  method: post\n  operationId: postInboxesByIdDraftsByDraftIdSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/drafts/{draftId}/send\n  method: post\n  operationId: postInboxesByIdDraftsByDraftIdSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/escalation\n  method: get\n  operationId: getInboxesByIdEscalation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/escalation\n  method: put\n  operationId: putInboxesByIdEscalation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/forwarding\n  method: get\n  operationId: getInboxesByIdForwarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/forwarding\n  method: post\n  operationId: postInboxesByIdForwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/forwarding/{forwardId}\n  method: delete\n  operationId: deleteInboxesByIdForwardingByForwardId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/forwarding/{forwardId}/resend\n  method: post\n  operationId: postInboxesByIdForwardingByForwardIdResend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/identity\n  method: get\n  operationId: getInboxesByIdIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/identity\n  method: patch\n  operationId: patchInboxesByIdIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/identity-token\n  method: post\n  operationId: postInboxesByIdIdentityToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/identity/sign-ins\n  method: get\n  operationId: getInboxesByIdIdentitySignIns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages\n  method: get\n  operationId: getInboxesByIdMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/messages/{messageId}/forward\n  method: post\n  operationId: postInboxesByIdMessagesByMessageIdForward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/messages/{messageId}/reply\n  method: post\n  operationId: postInboxesByIdMessagesByMessageIdReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/messages/claim\n  method: post\n  operationId: postInboxesByIdMessagesClaim\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/messages/send\n  method: post\n  operationId: postInboxesByIdMessagesSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/messages/wait\n  method: get\n  operationId: getInboxesByIdMessagesWait\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/pause\n  method: post\n  operationId: postInboxesByIdPause\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/resume\n  method: post\n  operationId: postInboxesByIdResume\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inboxes/{id}/threads\n  method: get\n  operationId: getInboxesByIdThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inboxes/{id}/verification\n\
  \  method: get\n  operationId: getInboxesByIdVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge\n  method: get\n  operationId: getKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge\n  method: post\n  operationId: postKnowledge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge/{id}\n  method: get\n  operationId: getKnowledgeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge/{id}\n\
  \  method: patch\n  operationId: patchKnowledgeById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge/{id}\n  method: delete\n  operationId: deleteKnowledgeById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge/search\n  method: get\n  operationId: getKnowledgeSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lists\n  method: get\n  operationId: getLists\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lists\n  method: post\n  operationId: postLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{id}\n  method: delete\n  operationId: deleteListsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/messages/{id}\n  method: get\n  operationId: getMessagesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/{id}\n  method: patch\n  operationId: patchMessagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/ack\n  method: post\n  operationId: postMessagesByIdAck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/attachments/{attachmentId}/extract\n\
  \  method: post\n  operationId: postMessagesByIdAttachmentsByAttachmentIdExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/attachments/{attachmentId}/text\n  method: get\n  operationId: getMessagesByIdAttachmentsByAttachmentIdText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/{id}/draft-reply\n  method: post\n  operationId: postMessagesByIdDraftReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/messages/{id}/extend\n  method: post\n  operationId: postMessagesByIdExtend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/nack\n  method: post\n  operationId: postMessagesByIdNack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/raw\n  method: get\n  operationId: getMessagesByIdRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/{id}/release\n\
  \  method: post\n  operationId: postMessagesByIdRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/batch-get\n  method: post\n  operationId: postMessagesBatchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/batch-update\n  method: post\n  operationId: postMessagesBatchUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (40 KB total) ---\n# Full source: https://artifacts.apis.io/agentboxd-com/agentic-access/agentboxd-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/agentboxd-com/agentic-access/agentboxd-com-agentic-access.yml
summary_line: 137 operations · 76 acting · 4 human-in-the-loop
tags:
- Artificial Intelligence
- Email
- Messaging
- Beta
---
