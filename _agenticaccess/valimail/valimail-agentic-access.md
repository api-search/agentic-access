---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 28
api_specs:
- filename: valimail-accounts-api-openapi.yml
  format: yaml
  label: Valimail Accounts API
  slug: valimail-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-accounts-api-openapi.yml
- filename: valimail-authentication-api-openapi.yml
  format: yaml
  label: Valimail Authentication API
  slug: valimail-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-authentication-api-openapi.yml
- filename: valimail-dkims-by-domain-api-openapi.yml
  format: yaml
  label: Valimail DKIMs by Domain API
  slug: valimail-dkims-by-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-dkims-by-domain-api-openapi.yml
- filename: valimail-dkims-by-sender-api-openapi.yml
  format: yaml
  label: Valimail DKIMs by Sender API
  slug: valimail-dkims-by-sender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-dkims-by-sender-api-openapi.yml
- filename: valimail-domains-api-openapi.yml
  format: yaml
  label: Valimail Domains API
  slug: valimail-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-domains-api-openapi.yml
- filename: valimail-mta-sts-policy-api-openapi.yml
  format: yaml
  label: Valimail MTA-STS Policy API
  slug: valimail-mta-sts-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-mta-sts-policy-api-openapi.yml
- filename: valimail-mta-sts-policy-reports-api-openapi.yml
  format: yaml
  label: Valimail MTA-STS Policy Reports API
  slug: valimail-mta-sts-policy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-mta-sts-policy-reports-api-openapi.yml
- filename: valimail-netblocks-api-openapi.yml
  format: yaml
  label: Valimail Netblocks API
  slug: valimail-netblocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-netblocks-api-openapi.yml
- filename: valimail-portfolios-api-openapi.yml
  format: yaml
  label: Valimail Portfolios API
  slug: valimail-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-portfolios-api-openapi.yml
- filename: valimail-scim-api-openapi.yml
  format: yaml
  label: Valimail SCIM API
  slug: valimail-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-scim-api-openapi.yml
- filename: valimail-senders-api-openapi.yml
  format: yaml
  label: Valimail Senders API
  slug: valimail-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-senders-api-openapi.yml
- filename: valimail-sso-api-openapi.yml
  format: yaml
  label: Valimail SSO API
  slug: valimail-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-sso-api-openapi.yml
- filename: valimail-tls-configuration-api-openapi.yml
  format: yaml
  label: Valimail TLS Configuration API
  slug: valimail-tls-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-tls-configuration-api-openapi.yml
- filename: valimail-users-api-openapi.yml
  format: yaml
  label: Valimail Users API
  slug: valimail-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-users-api-openapi.yml
- filename: valimail-webhooks-api-openapi.yml
  format: yaml
  label: Valimail Webhooks API
  slug: valimail-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/valimail-webhooks-api-openapi.yml
- filename: valimail-partner-openapi-original.yml
  format: yaml
  label: Valimail Partner API
  slug: valimail-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/openapi/_original/valimail-partner-openapi-original.yml
consequence_counts:
  physical: 9
  read: 28
  safety-critical: 1
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Valimail Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{slug}/v2
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{slug}/domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{slug}/domains/{domain}/dkims/{selector}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{slug}/domains/{domain}/netblocks/{netblock}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{slug}/domains/{domain}/senders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}/dkims
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}/dkims/{selector}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{slug}/users
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{slug}/users/{user-slug}/invitation
operation_count: 57
overview: 'Valimail exposes 57 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 19 write, 9 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Valimail
provider_slug: valimail
slug: valimail-agentic-access
source_filename: valimail-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/valimail-account-openapi-original.yml, openapi/valimail-config-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    acting: 29\n    connected: 28\n  by_consequence:\n    write: 19\n    read: 28\n    physical: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /auth\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/packages\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/users\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/users/{user-slug}/invitation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/users/{user-slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/users/{user-slug}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/v2\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /accounts/{slug}/v2/users/{user-slug}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/app/sso\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/app/sso\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/app/sso\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/app/sso\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/portfolios\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /webhooks/keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}\n  method: put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/senders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/senders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}/dkims\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}/dkims\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}/dkims/{selector}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/senders/{sender-slug}/dkims/{selector}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/dkims\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/dkims\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/dkims/{selector}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/dkims/{selector}\n\
  \  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/netblocks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/netblocks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/netblocks/{netblock}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/netblocks/{netblock}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/senders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/mta-sts/tls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/mta-sts/tls/summary\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/mta-sts/tls/failure-details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/mta_sts_policy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/mta_sts_policy\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/mta_sts_policy\n  method: put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/mta_sts_policies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/smtp_tls_policy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/domains/{domain}/smtp_tls_policy\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /accounts/{slug}/domains/{domain}/smtp_tls_policy\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/smtp_tls_policies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/scim/v2/Users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/scim/v2/Users\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{slug}/scim/v2/Users/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{slug}/scim/v2/Users/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valimail/refs/heads/main/agentic-access/valimail-agentic-access.yml
summary_line: 57 operations · 29 acting · 1 human-in-the-loop
tags:
- Email Authentication
- DMARC
- Email Security
- SPF
- DKIM
- BIMI
- MTA-STS
- Anti-Phishing
- Deliverability
- Cybersecurity
---
