---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 21
api_specs:
- filename: mail-in-a-box-dns-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box DNS API
  slug: mail-in-a-box-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-dns-api-openapi.yml
- filename: mail-in-a-box-mail-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box Mail API
  slug: mail-in-a-box-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-mail-api-openapi.yml
- filename: mail-in-a-box-mfa-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box MFA API
  slug: mail-in-a-box-mfa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-mfa-api-openapi.yml
- filename: mail-in-a-box-ssl-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box SSL API
  slug: mail-in-a-box-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-ssl-api-openapi.yml
- filename: mail-in-a-box-system-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box System API
  slug: mail-in-a-box-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-system-api-openapi.yml
- filename: mail-in-a-box-user-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box User API
  slug: mail-in-a-box-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-user-api-openapi.yml
- filename: mail-in-a-box-web-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box Web API
  slug: mail-in-a-box-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-web-api-openapi.yml
consequence_counts:
  physical: 1
  read: 21
  safety-critical: 2
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Mail In A Box Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mfa/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /system/reboot
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ssl/provision
operation_count: 49
overview: 'Mail-in-a-Box exposes 49 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 25 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mail-in-a-Box
provider_slug: mail-in-a-box
slug: mail-in-a-box-agentic-access
source_filename: mail-in-a-box-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/mailinabox-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 28\n    connected: 21\n  by_consequence:\n    write: 25\n    read: 21\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /system/status\n  method: post\n  operationId: getSystemStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/version\n  method: get\n  operationId: getSystemVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/latest-upstream-version\n  method: post\n  operationId: getSystemUpstreamVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/updates\n  method: get\n  operationId: getSystemUpdates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/update-packages\n  method: post\n  operationId: updateSystemPackages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /system/privacy\n  method: get\n  operationId: getSystemPrivacyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/privacy\n  method: post\n  operationId: updateSystemPrivacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /system/reboot\n  method: get\n  operationId: getSystemRebootStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/reboot\n  method: post\n  operationId: rebootSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /system/backup/status\n  method: get\n  operationId: getSystemBackupStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/backup/config\n  method: get\n  operationId: getSystemBackupConfig\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/backup/config\n  method: post\n  operationId: updateSystemBackupConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ssl/status\n  method: get\n  operationId: getSSLStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ssl/csr/{domain}\n  method: post\n  operationId: generateSSLCSR\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /ssl/install\n  method: post\n  operationId: installSSLCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ssl/provision\n  method: post\n  operationId: provisionSSLCertificates\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/secondary-nameserver\n  method: get\n  operationId: getDnsSecondaryNameserver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/secondary-nameserver\n  method: post\n  operationId: addDnsSecondaryNameserver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/zones\n  method: get\n  operationId: getDnsZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/zonefile/{zone}\n  method: get\n  operationId: getDnsZonefile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/update\n  method: post\n  operationId: updateDns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/custom\n  method: get\n  operationId: getDnsCustomRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/custom/{qname}/{rtype}\n  method: get\n  operationId: getDnsCustomRecordsForQNameAndType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/custom/{qname}/{rtype}\n  method: post\n  operationId: addDnsCustomRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /dns/custom/{qname}/{rtype}\n  method: put\n  operationId: updateDnsCustomRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/custom/{qname}/{rtype}\n  method: delete\n  operationId: removeDnsCustomRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/custom/{qname}\n  method: get\n  operationId: getDnsCustomARecordsForQName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/custom/{qname}\n\
  \  method: post\n  operationId: addDnsCustomARecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/custom/{qname}\n  method: put\n  operationId: updateDnsCustomARecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/custom/{qname}\n  method: delete\n  operationId: removeDnsCustomARecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /dns/dump\n  method: get\n  operationId: getDnsDump\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mail/users\n  method: get\n  operationId: getMailUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mail/users/add\n  method: post\n  operationId: addMailUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail/users/remove\n  method: post\n  operationId: removeMailUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail/users/privileges/add\n  method: post\n  operationId: addMailUserPrivilege\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail/users/privileges/remove\n  method: post\n  operationId: removeMailUserPrivilege\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail/users/password\n  method: post\n  operationId: setMailUserPassword\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail/users/privileges\n  method: get\n  operationId: getMailUserPrivileges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mail/domains\n  method: get\n  operationId: getMailDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mail/aliases\n  method: get\n  operationId: getMailAliases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mail/aliases/add\n  method: post\n  operationId: upsertMailAlias\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail/aliases/remove\n  method: post\n  operationId: removeMailAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/domains\n  method: get\n  operationId: getWebDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/update\n  method: post\n  operationId: updateWeb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mfa/status\n  method: post\n  operationId: mfaStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mfa/totp/enable\n  method: post\n  operationId: mfaTotpEnable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mfa/disable\n  method: post\n  operationId: mfaTotpDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/mail-in-a-box/agentic-access/mail-in-a-box-agentic-access.yml
summary_line: 49 operations · 28 acting · 2 human-in-the-loop
tags:
- Company
- Email
- Self-Hosted
- Open Source
- Automation
- Privacy
---
