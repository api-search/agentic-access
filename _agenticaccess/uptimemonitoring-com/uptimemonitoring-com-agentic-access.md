---
acting_count: 47
action_class_counts:
  acting: 47
  connected: 51
api_specs:
- filename: uptimemonitoring-com-account-api-openapi.yml
  format: yaml
  label: Monitive Account API
  slug: uptimemonitoring-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-account-api-openapi.yml
- filename: uptimemonitoring-com-admin-api-openapi.yml
  format: yaml
  label: Monitive Admin API
  slug: uptimemonitoring-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-admin-api-openapi.yml
- filename: uptimemonitoring-com-announcements-api-openapi.yml
  format: yaml
  label: Monitive Announcements API
  slug: uptimemonitoring-com-announcements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-announcements-api-openapi.yml
- filename: uptimemonitoring-com-email-api-openapi.yml
  format: yaml
  label: Monitive Email API
  slug: uptimemonitoring-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-email-api-openapi.yml
- filename: uptimemonitoring-com-events-api-openapi.yml
  format: yaml
  label: Monitive Events API
  slug: uptimemonitoring-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-events-api-openapi.yml
- filename: uptimemonitoring-com-feed-api-openapi.yml
  format: yaml
  label: Monitive Feed API
  slug: uptimemonitoring-com-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-feed-api-openapi.yml
- filename: uptimemonitoring-com-feed-xml-api-openapi.yml
  format: yaml
  label: Monitive Feed.xml API
  slug: uptimemonitoring-com-feed-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-feed-xml-api-openapi.yml
- filename: uptimemonitoring-com-incidents-api-openapi.yml
  format: yaml
  label: Monitive Incidents API
  slug: uptimemonitoring-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-incidents-api-openapi.yml
- filename: uptimemonitoring-com-keys-api-openapi.yml
  format: yaml
  label: Monitive Keys API
  slug: uptimemonitoring-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-keys-api-openapi.yml
- filename: uptimemonitoring-com-monitors-api-openapi.yml
  format: yaml
  label: Monitive Monitors API
  slug: uptimemonitoring-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-monitors-api-openapi.yml
- filename: uptimemonitoring-com-oauth-api-openapi.yml
  format: yaml
  label: Monitive OAuth API
  slug: uptimemonitoring-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-oauth-api-openapi.yml
- filename: uptimemonitoring-com-public-api-openapi.yml
  format: yaml
  label: Monitive Public API
  slug: uptimemonitoring-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-public-api-openapi.yml
- filename: uptimemonitoring-com-push-api-openapi.yml
  format: yaml
  label: Monitive Push API
  slug: uptimemonitoring-com-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-push-api-openapi.yml
- filename: uptimemonitoring-com-recipients-api-openapi.yml
  format: yaml
  label: Monitive Recipients API
  slug: uptimemonitoring-com-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-recipients-api-openapi.yml
- filename: uptimemonitoring-com-webhook-deliveries-api-openapi.yml
  format: yaml
  label: Monitive Webhook Deliveries API
  slug: uptimemonitoring-com-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-webhook-deliveries-api-openapi.yml
consequence_counts:
  physical: 2
  read: 51
  safety-critical: 7
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Uptimemonitoring Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/account/feed-token/rotate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/invites/{inviteID}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/admin/kill-switch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/admin/kill-switch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/monitors/{monitorID}/test
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/push/subscribe/{subscriptionID}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/recipients/{recipientID}/confirm/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/recipients/{recipientID}/test
operation_count: 98
overview: 'Monitive exposes 98 API operations that an AI agent could call, of which 47 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 51 read, 38 write, 2 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Monitive
provider_slug: uptimemonitoring-com
slug: uptimemonitoring-com-agentic-access
source_filename: uptimemonitoring-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/uptimemonitoring-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 98\n  by_action_class:\n    connected: 51\n    acting: 47\n  by_consequence:\n    read: 51\n    write: 38\n    safety-critical: 7\n    physical: 2\n  human_in_the_loop_required: 7\noperations:\n- path: /\n  method: get\n  operationId: getServiceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /oauth/github/login\n  method: get\n  operationId: oauthGitHubLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/github/callback\n  method: get\n  operationId: oauthGitHubCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/github/link\n  method: post\n  operationId: oauthGitHubLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/exchange\n  method: post\n  operationId: oauthExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/email/start\n  method: post\n  operationId: oauthEmailStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/email/verify\n  method: post\n  operationId: oauthEmailVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/google/login\n  method: get\n  operationId: oauthGoogleLogin\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/google/link\n  method: post\n  operationId: oauthGoogleLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/google/callback\n  method: get\n  operationId: oauthGoogleCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: oauthPRM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: oauthASMetadata\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/register\n  method: post\n  operationId: oauthRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/authorize\n  method: get\n  operationId: oauthAuthorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token\n  method: post\n  operationId: oauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /oauth2/revoke\n  method: post\n  operationId: oauthRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth2/keys\n  method: get\n  operationId: oauthJWKS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/{keyID}\n  method: delete\n  operationId: deleteKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/{keyID}/rotate\n  method: post\n  operationId: rotateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/monitors\n  method: get\n  operationId: listMonitors\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monitors\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/monitors/{monitorID}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monitors/{monitorID}\n  method: put\n  operationId: updateMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/monitors/{monitorID}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/incidents\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/incidents/{incidentID}\n  method: get\n  operationId: getIncident\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/v1/me/account\n  method: post\n  operationId: switchAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/reports\n  method: get\n  operationId: getReportPrefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/reports\n  method: patch\n  operationId: setReportPrefs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/identities/github\n\
  \  method: post\n  operationId: startGitHubLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/invites\n  method: get\n  operationId: listMyInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/invites/{inviteID}/accept\n  method: post\n  operationId: acceptInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/invites\n  method: post\n  operationId: createInvite\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/invites\n  method: get\n  operationId: listInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/invites/{inviteID}\n  method: delete\n  operationId: revokeInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/me/identities/google\n  method: post\n  operationId: startGoogleLink\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/identities/email/start\n  method: post\n  operationId: startEmailLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/identities/email/verify\n  method: post\n  operationId: verifyEmailLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account\n\
  \  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account\n  method: patch\n  operationId: patchAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/usage\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/events\n  method: get\n  operationId: listAccountEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/announcements\n\
  \  method: get\n  operationId: listAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/announcements\n  method: post\n  operationId: createAnnouncement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/announcements/{announcementID}\n  method: put\n  operationId: updateAnnouncement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/announcements/{announcementID}\n  method: delete\n  operationId:\
  \ deleteAnnouncement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/monitors/{monitorID}/webhook\n  method: get\n  operationId: getMonitorWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monitors/{monitorID}/webhook\n  method: put\n  operationId: putMonitorWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/monitors/{monitorID}/webhook\n  method: delete\n  operationId: deleteMonitorWebhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients\n  method: get\n  operationId: listRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recipients\n  method: post\n  operationId: createRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients/{recipientID}\n  method: get\n  operationId: getRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recipients/{recipientID}\n  method: patch\n  operationId: patchRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients/{recipientID}\n  method: delete\n  operationId: deleteRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients/{recipientID}/confirm/resend\n  method: post\n  operationId: resendRecipientConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients/{recipientID}/test\n  method: post\n  operationId: testRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/confirm/{token}\n  method: get\n  operationId: confirmEmailRecipientPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/confirm/{token}\n  method: post\n  operationId: confirmEmailRecipient\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/unsubscribe/{token}\n  method: get\n  operationId: unsubscribeRecipientPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/unsubscribe/{token}\n  method: post\n  operationId: unsubscribeRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/reports/{type}/unsubscribe/{token}\n  method: get\n  operationId: reportUnsubscribePage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/reports/{type}/unsubscribe/{token}\n  method: post\n  operationId: reportUnsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/monitors/{monitorID}/recipients\n  method: get\n  operationId: getMonitorRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monitors/{monitorID}/recipients\n  method: put\n  operationId: putMonitorRecipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/monitors/{monitorID}/uptime\n  method: get\n  operationId: getMonitorUptime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monitors/{monitorID}/status-page\n  method: get\n  operationId: getMonitorStatusPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monitors/{monitorID}/status-page\n  method: put\n  operationId: setMonitorStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/monitors/{monitorID}/test\n  method: post\n  operationId: testMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/webhook-deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed/{token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed.xml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /feed/{token}/rss\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/feed-token\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/feed-token/rotate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/events/ticket\n  method: post\n  operationId: issueSSETicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/events/stream\n  method: get\n  operationId: subscribeSSEStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/push/subscribe\n  method: post\n  operationId: subscribeBrowserPush\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/push/subscribe/{subscriptionID}\n  method: delete\n  operationId: unsubscribeBrowserPush\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n     \
  \ proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/push/subscriptions\n  method: get\n  operationId: listBrowserPushSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/ping\n  method: get\n  operationId: adminPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/kill-switch\n  method: get\n  operationId: adminKillSwitchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/kill-switch\n  method: post\n  operationId: adminKillSwitchEngage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/admin/kill-switch\n  method: delete\n  operationId: adminKillSwitchDisengage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/admin/scheduler/transition-drops\n  method: get\n  operationId: adminSchedulerTransitionDrops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/events/ticket\n  method: post\n  operationId: issueAdminSSETicket\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/events/stream\n  method: get\n  operationId: subscribeAdminSSEStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/monitors/state\n  method: get\n  operationId: adminMonitorsState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/monitors/{accountID}/{monitorID}/meta\n  method: get\n  operationId: adminMonitorMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/push/vapid-public-key\n  method: get\n  operationId:\
  \ getBrowserPushVapidPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}\n  method: get\n  operationId: getStatusPageHTML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/feed.rss\n  method: get\n  operationId: getStatusPageRSS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/feed.atom\n  method: get\n  operationId: getStatusPageAtom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/status.json\n  method: get\n  operationId: getStatusPageJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/badge.svg\n  method: get\n  operationId: getStatusPageBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/uptimemonitoring-com/agentic-access/uptimemonitoring-com-agentic-access.yml
summary_line: 98 operations · 47 acting · 7 human-in-the-loop
tags:
- Uptime Monitoring
- API-First
- Developer Tools
- Observability
- Software-as-a-Service
---
