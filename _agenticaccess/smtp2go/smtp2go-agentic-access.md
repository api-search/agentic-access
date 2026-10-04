---
acting_count: 68
action_class_counts:
  acting: 68
  connected: 5
api_specs:
- filename: smtp2go-activity-api-openapi.yml
  format: yaml
  label: SMTP2GO Activity API
  slug: smtp2go-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-activity-api-openapi.yml
- filename: smtp2go-api-keys-api-openapi.yml
  format: yaml
  label: SMTP2GO API Keys API
  slug: smtp2go-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-api-keys-api-openapi.yml
- filename: smtp2go-sms-api-openapi.yml
  format: yaml
  label: SMTP2GO SMS API
  slug: smtp2go-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-sms-api-openapi.yml
- filename: smtp2go-smtp-users-api-openapi.yml
  format: yaml
  label: SMTP2GO SMTP Users API
  slug: smtp2go-smtp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-smtp-users-api-openapi.yml
- filename: smtp2go-subaccounts-api-openapi.yml
  format: yaml
  label: SMTP2GO Subaccounts API
  slug: smtp2go-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-subaccounts-api-openapi.yml
- filename: smtp2go-suppressions-api-openapi.yml
  format: yaml
  label: SMTP2GO Suppressions API
  slug: smtp2go-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-suppressions-api-openapi.yml
- filename: smtp2go-templates-api-openapi.yml
  format: yaml
  label: SMTP2GO Templates API
  slug: smtp2go-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-templates-api-openapi.yml
- filename: smtp2go-webhooks-api-openapi.yml
  format: yaml
  label: SMTP2GO Webhooks API
  slug: smtp2go-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-webhooks-api-openapi.yml
- filename: smtp2go-allowed-recipients-api-openapi.yml
  format: yaml
  label: SMTP2GO ALLOWED RECIPIENTS API
  slug: smtp2go-allowed-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-allowed-recipients-api-openapi.yml
- filename: smtp2go-allowed-senders-api-openapi.yml
  format: yaml
  label: SMTP2GO ALLOWED SENDERS API
  slug: smtp2go-allowed-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-allowed-senders-api-openapi.yml
- filename: smtp2go-dedicated-ips-api-openapi.yml
  format: yaml
  label: SMTP2GO DEDICATED IPS API
  slug: smtp2go-dedicated-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-dedicated-ips-api-openapi.yml
- filename: smtp2go-email-archive-api-openapi.yml
  format: yaml
  label: SMTP2GO EMAIL ARCHIVE API
  slug: smtp2go-email-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-email-archive-api-openapi.yml
- filename: smtp2go-emails-api-openapi.yml
  format: yaml
  label: SMTP2GO EMAILS API
  slug: smtp2go-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-emails-api-openapi.yml
- filename: smtp2go-ip-auth-api-openapi.yml
  format: yaml
  label: SMTP2GO IP AUTH API
  slug: smtp2go-ip-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-ip-auth-api-openapi.yml
- filename: smtp2go-sender-domains-api-openapi.yml
  format: yaml
  label: SMTP2GO SENDER DOMAINS API
  slug: smtp2go-sender-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-sender-domains-api-openapi.yml
- filename: smtp2go-single-sender-emails-api-openapi.yml
  format: yaml
  label: SMTP2GO SINGLE SENDER EMAILS API
  slug: smtp2go-single-sender-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-single-sender-emails-api-openapi.yml
- filename: smtp2go-statistics-api-openapi.yml
  format: yaml
  label: SMTP2GO STATISTICS API
  slug: smtp2go-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-statistics-api-openapi.yml
- filename: smtp2go-ip-allowlist-api-openapi.yml
  format: yaml
  label: SMTP2GO IP Allowlist API
  slug: smtp2go-ip-allowlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-ip-allowlist-api-openapi.yml
consequence_counts:
  physical: 18
  read: 5
  write: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smtp2Go Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /allowed_senders/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /allowed_senders/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /allowed_senders/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /allowed_senders/view
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/returnpath
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/subaccount_access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/tracking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domain/view
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/mime
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /single_sender_emails/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /single_sender_emails/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /single_sender_emails/view
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/send
operation_count: 73
overview: 'SMTP2GO exposes 73 API operations that an AI agent could call, of which 68 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 50 write, and 18 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SMTP2GO
provider_slug: smtp2go
slug: smtp2go-agentic-access
source_filename: smtp2go-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/smtp2go-activity-api-openapi.yml, openapi/smtp2go-allowed-recipients-api-openapi.yml,\n  openapi/smtp2go-allowed-senders-api-openapi.yml, openapi/smtp2go-api-keys-api-openapi.yml,\n  openapi/smtp2go-dedicated-ips-api-openapi.yml, openapi/smtp2go-email-archive-api-openapi.yml,\n  openapi/smtp2go-emails-api-openapi.yml, openapi/smtp2go-ip-allowlist-api-openapi.yml, openapi/smtp2go-ip-auth-api-openapi.yml,\n  openapi/smtp2go-sender-domains-api-openapi.yml, openapi/smtp2go-single-sender-emails-api-openapi.yml,\n  openapi/smtp2go-sms-api-openapi.yml, openapi/smtp2go-smtp-users-api-openapi.yml, openapi/smtp2go-statistics-api-openapi.yml,\n  openapi/smtp2go-subaccounts-api-openapi.yml, openapi/smtp2go-suppressions-api-openapi.yml,\n  openapi/smtp2go-templates-api-openapi.yml, openapi/smtp2go-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI.\
  \ A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 73\n  by_action_class:\n    connected: 5\n    acting: 68\n  by_consequence:\n    read: 5\n    write: 50\n    physical: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /activity/search\n  method: post\n  operationId: search-activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allowed_recipients/add\n  method: post\n  operationId: add-allowed-recipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allowed_recipients/remove\n  method: post\n  operationId: remove-allowed-recipients\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allowed_recipients/update\n  method: post\n  operationId: update-allowed-recipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allowed_recipients/view\n  method: post\n  operationId: view-allowed-recipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /allowed_senders/add\n  method: post\n  operationId: add-allowed-senders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allowed_senders/remove\n  method: post\n  operationId: remove-allowed-senders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allowed_senders/update\n  method: post\n  operationId: update-allowed-senders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allowed_senders/view\n  method: post\n  operationId: view-allowed-senders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/add\n  method: post\n  operationId: add-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api_keys/edit\n  method: post\n  operationId: edit-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/edit\n  method: patch\n  operationId: patch-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/permissions\n  method: post\n  operationId: view-api-key-permissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/remove\n  method: post\n  operationId: remove-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/view\n  method: post\n  operationId: view-api-keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_ips/view\n  method: post\n  operationId: view-dedicated-ips\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /archive/email\n  method: post\n  operationId: view-an-archived-email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /archive/search\n  method: post\n  operationId: search-archived-pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/batch\n  method: post\n  operationId: send-email-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/mime\n  method: post\n  operationId: send-mime-email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/scheduled/remove\n  method: post\n  operationId: remove-scheduled-email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/scheduled/search\n  method: post\n  operationId: search-scheduled-emails\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/send\n  method: post\n  operationId: send-standard-email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_allow_list\n  method: post\n  operationId: ip-allowlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_allow_list/add\n  method: post\n  operationId: add-ip-allowlist\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_allow_list/edit\n  method: post\n  operationId: edit-ip-allowlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_allow_list/remove\n  method: post\n  operationId: remove-ip-allowlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_allow_list/view\n  method: post\n  operationId: view-ip-allowlist\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_auth/edit\n  method: patch\n  operationId: patch-ip-auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_auth/remove\n  method: post\n  operationId: remove-ip-auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_auth/view\n  method:\
  \ post\n  operationId: view-ip-auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/add\n  method: post\n  operationId: add-sender-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/remove\n  method: post\n  operationId: remove-sender-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/returnpath\n  method: post\n  operationId: edit-return-path-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/subaccount_access\n  method: post\n  operationId: edit-subaccount-access\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/tracking\n  method: post\n  operationId:\
  \ edit-tracking-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/verify\n  method: post\n  operationId: verify-a-sender-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain/view\n  method: post\n  operationId: view-sender-domains\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /single_sender_emails/add\n  method: post\n  operationId: add-a-single-sender-email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /single_sender_emails/remove\n  method: post\n  operationId: remove-a-single-sender-email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /single_sender_emails/view\n  method: post\n  operationId: view-all-single-sender-emails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/send\n  method: post\n  operationId: send-sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/summary\n  method: post\n  operationId: sms-summary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/view-received\n  method: post\n  operationId: view-received-sms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/view-sent\n  method: post\n  operationId: view-sent-sms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/smtp/add\n  method: post\n  operationId: add-an-smtp-user\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/smtp/edit\n  method: post\n  operationId: edit-an-smtp-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/smtp/edit\n  method: patch\n  operationId: patch-smtp-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/smtp/remove\n  method: post\n  operationId: remove-an-smtp-user\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/smtp/view\n  method: post\n  operationId: view-smtp-users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/email_bounces\n  method: post\n  operationId: email-bounces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/email_cycle\n\
  \  method: post\n  operationId: email-cycle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/email_history\n  method: post\n  operationId: email-history\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/email_spam\n  method: post\n  operationId: email-spam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /stats/email_summary\n  method: post\n  operationId: email-summary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/email_unsubs\n  method: post\n  operationId: email-unsubscribes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccount/add\n  method: post\n  operationId: add-subaccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccount/close\n  method: post\n  operationId: close-a-subaccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccount/edit\n  method: post\n  operationId: update-a-subaccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccount/reopen\n  method: post\n  operationId: reopen-a-closed-subaccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccounts/search\n  method: post\n  operationId: search-subaccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppression/add\n  method: post\n  operationId: add-a-suppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppression/remove\n  method: post\n  operationId: remove-a-suppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppression/view\n  method: post\n  operationId: view-suppressions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/add\n  method: post\n  operationId: add-an-email-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/delete\n  method: post\n  operationId: remove-an-email-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/edit\n  method: post\n  operationId: update-an-email-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/search\n  method: post\n  operationId: search-email-templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /template/view\n  method: post\n  operationId: view-template-details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/add\n  method: post\n  operationId: add-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/edit\n  method: post\n  operationId: edit-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/remove\n  method: post\n  operationId: remove-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/view\n  method: post\n  operationId: view-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/agentic-access/smtp2go-agentic-access.yml
summary_line: 73 operations · 68 acting
tags:
- Email
- Email Delivery
- Transactional Email
- SMTP
- SMS
- Email API
- Deliverability
- Webhook
- Messaging
- Communications
- MCP
- Agent Skills
---
