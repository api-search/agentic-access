---
acting_count: 57
action_class_counts:
  acting: 57
  connected: 30
api_specs:
- filename: timescale-analytics-api-openapi.yml
  format: yaml
  label: Timescale Analytics API
  slug: timescale-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-analytics-api-openapi.yml
- filename: timescale-auth-api-openapi.yml
  format: yaml
  label: Timescale Auth API
  slug: timescale-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-auth-api-openapi.yml
- filename: timescale-feedback-api-openapi.yml
  format: yaml
  label: Timescale Feedback API
  slug: timescale-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-feedback-api-openapi.yml
- filename: timescale-health-api-openapi.yml
  format: yaml
  label: Timescale Health API
  slug: timescale-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-health-api-openapi.yml
- filename: timescale-invites-api-openapi.yml
  format: yaml
  label: Timescale Invites API
  slug: timescale-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-invites-api-openapi.yml
- filename: timescale-pricing-api-openapi.yml
  format: yaml
  label: Timescale Pricing API
  slug: timescale-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-pricing-api-openapi.yml
- filename: timescale-projects-api-openapi.yml
  format: yaml
  label: Timescale Projects API
  slug: timescale-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-projects-api-openapi.yml
- filename: timescale-read-replica-sets-api-openapi.yml
  format: yaml
  label: Timescale Read Replica Sets API
  slug: timescale-read-replica-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-read-replica-sets-api-openapi.yml
- filename: timescale-services-api-openapi.yml
  format: yaml
  label: Timescale Services API
  slug: timescale-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-services-api-openapi.yml
- filename: timescale-spaces-api-openapi.yml
  format: yaml
  label: Timescale Spaces API
  slug: timescale-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-spaces-api-openapi.yml
- filename: timescale-vpcs-api-openapi.yml
  format: yaml
  label: Timescale VP Cs API
  slug: timescale-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-vpcs-api-openapi.yml
consequence_counts:
  physical: 4
  read: 30
  safety-critical: 5
  write: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Timescale Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /projects/{project_id}/services/{service_id}/disablePooler
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /projects/{project_id}/services/{service_id}/replicaSets/{replica_set_id}/disablePooler
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /projects/{project_id}/services/{service_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /spaces/{space_id}/shares/{share_token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spaces/{space_id}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /spaces/{space_id}/payment/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /spaces/{space_id}/payment/{payment_id}/deletion
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /spaces/{space_id}/payment/{payment_id}/primary
operation_count: 87
overview: 'Timescale exposes 87 API operations that an AI agent could call, of which 57 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 48 write, 4 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Timescale
provider_slug: timescale
slug: timescale-agentic-access
source_filename: timescale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/timescale-ghost-openapi-original.yml, openapi/timescale-tiger-cloud-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 87\n  by_action_class:\n    connected: 30\n    acting: 57\n  by_consequence:\n    read: 30\n    write: 48\n    safety-critical: 5\n    physical: 4\n  human_in_the_loop_required: 5\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/info\n  method: get\n  operationId: authInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces\n  method: get\n  operationId: listSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/rename\n  method: post\n  operationId: renameSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/usage\n  method: get\n  operationId: spaceUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/status\n  method: get\n  operationId: spaceStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/members/{user_id}\n  method: delete\n  operationId: removeMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/members/{user_id}/role\n  method: put\n  operationId: updateMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/leave\n  method: post\n  operationId: leaveSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/invites\n  method: get\n  operationId: listInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/invites\n  method: post\n  operationId: createInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/invites/{email}\n  method: delete\n  operationId: cancelInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites\n  method: get\n  operationId: listReceivedInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invites/{space_id}/accept\n  method: post\n  operationId: acceptInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /invites/{space_id}/decline\n  method: post\n  operationId: declineInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/api_keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/api_keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/api_keys/{prefix}\n  method: delete\n\
  \  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases\n  method: get\n  operationId: listDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/databases\n  method: post\n  operationId: createDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}\n  method: get\n  operationId: getDatabase\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/databases/{database_ref}\n  method: delete\n  operationId: deleteDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}/fork\n  method: post\n  operationId: forkDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}/pause\n  method: post\n  operationId: pauseDatabase\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}/resume\n  method: post\n  operationId: resumeDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}/rename\n  method: post\n  operationId: renameDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}/password\n  method: post\n  operationId: updatePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/databases/{database_ref}/logs\n  method: get\n  operationId: databaseLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/databases/{database_ref}/share\n  method: post\n  operationId: shareDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /spaces/{space_id}/shares\n  method: get\n  operationId: listShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/shares/{share_token}\n  method: delete\n  operationId: revokeShare\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /spaces/{space_id}/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/invoices/{invoice_id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/payment\n  method: get\n  operationId: listPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/payment\n  method: post\n  operationId: createPaymentMethodSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/payment/{payment_id}\n  method: get\n  operationId: getPaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /spaces/{space_id}/payment/{payment_id}\n  method: delete\n  operationId: deletePaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/payment/{payment_id}/primary\n  method: put\n  operationId: setPaymentMethodPrimary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/payment/{payment_id}/deletion\n  method: delete\n  operationId: cancelPaymentMethodDeletion\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{space_id}/overages\n  method: put\n  operationId: updateOverages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/identify\n  method: post\n  operationId: analyticsIdentify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /analytics/track\n  method: post\n  operationId: analyticsTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/info\n  method: get\n  operationId: getAuthInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/logout\n  method: post\n  operationId: logout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /analytics/identify\n  method: post\n  operationId: identifyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/track\n  method: post\n  operationId: trackEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/vpcs\n  method: get\n  operationId: getVPCs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/vpcs\n  method: post\n  operationId: createVPC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/vpcs/{vpc_id}\n  method: get\n  operationId: getVPC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /projects/{project_id}/vpcs/{vpc_id}\n  method: delete\n  operationId: deleteVPC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/vpcs/{vpc_id}/rename\n  method: post\n  operationId: renameVPC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/vpcs/{vpc_id}/peerings\n  method: get\n  operationId: getVPCPeerings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /projects/{project_id}/vpcs/{vpc_id}/peerings\n  method: post\n  operationId: createVPCPeering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/vpcs/{vpc_id}/peerings/{peering_id}\n  method: get\n  operationId: getVPCPeering\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/vpcs/{vpc_id}/peerings/{peering_id}\n  method: delete\n  operationId: deleteVPCPeering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /projects/{project_id}/services\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/services\n  method: post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/services/{service_id}\n  method: delete\n  operationId: deleteService\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/start\n  method: post\n  operationId: startService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/stop\n  method: post\n  operationId: stopService\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/attachToVPC\n  method: post\n  operationId: attachServiceToVPC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/detachFromVPC\n  method: post\n  operationId: detachServiceFromVPC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/resize\n  method: post\n  operationId: resizeService\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/enablePooler\n  method: post\n  operationId: enablePooler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/disablePooler\n  method: post\n  operationId: disablePooler\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/forkService\n  method: post\n  operationId: forkService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/updatePassword\n  method: post\n  operationId: updatePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/setEnvironment\n  method: post\n  operationId: setEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/logs\n  method: get\n  operationId: getServiceLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/services/{service_id}/metrics/available-series\n  method: get\n  operationId: getServiceMetricsAvailableSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/services/{service_id}/metrics/series\n  method: post\n  operationId: getServiceMetricsSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/setHA\n  method: post\n  operationId: setHAReplica\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/replicaSets\n  method: get\n  operationId: getReplicaSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/services/{service_id}/replicaSets\n  method: post\n  operationId: createReplicaSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/replicaSets/{replica_set_id}\n  method: delete\n  operationId: deleteReplicaSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/replicaSets/{replica_set_id}/resize\n  method: post\n  operationId: resizeReplicaSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /projects/{project_id}/services/{service_id}/replicaSets/{replica_set_id}/enablePooler\n  method: post\n  operationId: enableReplicaPooler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/replicaSets/{replica_set_id}/disablePooler\n  method: post\n  operationId: disableReplicaPooler\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /projects/{project_id}/services/{service_id}/replicaSets/{replica_set_id}/setEnvironment\n\
  \  method: post\n  operationId: setReplicaEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/agentic-access/timescale-agentic-access.yml
summary_line: 87 operations · 57 acting · 5 human-in-the-loop
tags:
- Company
- Database
- PostgreSQL
- Time Series
- Analytics
- Cloud Infrastructure
- Data Platform
- Vector Search
- Developer Tools
- Open-Source
---
