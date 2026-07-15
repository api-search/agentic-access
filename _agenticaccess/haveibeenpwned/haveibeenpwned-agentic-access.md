---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 14
api_specs:
- filename: hibp-openapi.yml
  format: yaml
  label: HIBP API v3
  slug: hibp-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/hibp-openapi.yml
- filename: pwned-passwords-openapi.yml
  format: yaml
  label: Pwned Passwords
  slug: pwned-passwords
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/openapi/pwned-passwords-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Haveibeenpwned Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainverification/sendEmail
operation_count: 17
overview: 'HaveIBeenPwned exposes 17 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HaveIBeenPwned
provider_slug: haveibeenpwned
slug: haveibeenpwned-agentic-access
source_filename: haveibeenpwned-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hibp-openapi.yml, openapi/pwned-passwords-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 14\n    acting: 3\n  by_consequence:\n    read: 14\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /breachedaccount/{account}\n  method: get\n  operationId: getBreachesForAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breachedaccount/range/{hashPrefix}\n  method: get\n  operationId: getBreachesByRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /breaches\n  method: get\n  operationId: listBreaches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breach/{name}\n  method: get\n  operationId: getBreachByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latestbreach\n  method: get\n  operationId: getLatestBreach\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataclasses\n  method: get\n  operationId: listDataClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pasteaccount/{account}\n  method: get\n  operationId: getPastesForAccount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stealerlogsbyemail/{email}\n  method: get\n  operationId: getStealerLogsByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stealerlogsbywebsitedomain/{domain}\n  method: get\n  operationId: getStealerLogsByWebsiteDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stealerlogsbyemaildomain/{domain}\n  method: get\n  operationId: getStealerLogsByEmailDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breacheddomain/{domain}\n  method: get\n  operationId: getBreachedDomain\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribeddomains\n  method: get\n  operationId: listSubscribedDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainverification/generateDnsToken\n  method: post\n  operationId: generateDnsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainverification/verifyDnsToken\n  method: post\n  operationId: verifyDnsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /domainverification/sendEmail\n  method: post\n  operationId: sendDomainVerificationEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/status\n  method: get\n  operationId: getSubscriptionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /range/{hashPrefix}\n  method: get\n  operationId: searchPasswordRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haveibeenpwned/refs/heads/main/agentic-access/haveibeenpwned-agentic-access.yml
summary_line: 17 operations · 3 acting
tags:
- Security
- Breach Notification
- Credential Stuffing
- Stealer Logs
- K-Anonymity
- Privacy
- Identity
---
