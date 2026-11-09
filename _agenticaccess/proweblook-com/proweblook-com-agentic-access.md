---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 23
api_specs:
- filename: proweblook-com-account-api-openapi.yml
  format: yaml
  label: proweblook-com Account API
  slug: proweblook-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-account-api-openapi.yml
- filename: proweblook-com-ai-audit-api-openapi.yml
  format: yaml
  label: proweblook-com AI Audit API
  slug: proweblook-com-ai-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-ai-audit-api-openapi.yml
- filename: proweblook-com-email-api-openapi.yml
  format: yaml
  label: proweblook-com Email API
  slug: proweblook-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-email-api-openapi.yml
- filename: proweblook-com-ip-api-openapi.yml
  format: yaml
  label: proweblook-com IP API
  slug: proweblook-com-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-ip-api-openapi.yml
- filename: proweblook-com-phone-api-openapi.yml
  format: yaml
  label: proweblook-com Phone API
  slug: proweblook-com-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-phone-api-openapi.yml
- filename: proweblook-com-scraping-api-openapi.yml
  format: yaml
  label: proweblook-com Scraping API
  slug: proweblook-com-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-scraping-api-openapi.yml
- filename: proweblook-com-security-api-openapi.yml
  format: yaml
  label: proweblook-com Security API
  slug: proweblook-com-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-security-api-openapi.yml
- filename: proweblook-com-system-api-openapi.yml
  format: yaml
  label: proweblook-com System API
  slug: proweblook-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-system-api-openapi.yml
- filename: proweblook-com-whats-app-api-openapi.yml
  format: yaml
  label: proweblook-com Whats App API
  slug: proweblook-com-whats-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/proweblook-com/openapi/proweblook-com-whats-app-api-openapi.yml
consequence_counts:
  read: 23
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Proweblook Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'proweblook-com exposes 29 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: proweblook-com
provider_slug: proweblook-com
slug: proweblook-com-agentic-access
source_filename: proweblook-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/proweblook-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 23\n    acting: 6\n  by_consequence:\n    read: 23\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: checkGeoIP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkwanumber\n  method: get\n  operationId: checkWhatsAppNumber\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonevalidation\n  method: get\n  operationId: validatePhoneNumberGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonevalidation\n  method: post\n  operationId: validatePhoneNumberPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: get\n  operationId: checkBlacklistMonolith\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailvalidation\n  method: get\n  operationId:\
  \ verifyEmailLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkemail\n  method: get\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkemailcron\n  method: get\n  operationId: verifyEmailCronCompatible\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkgeoip\n  method: get\n  operationId: checkGeoIPCompatible\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkbalance\n  method: get\n  operationId: checkBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /sendwasms\n  method: get\n  operationId: sendWhatsAppMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scrapersearch\n  method: get\n  operationId: searchReddit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scraperpost\n  method: get\n  operationId: scrapeRedditPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scraperxsearch\n  method: get\n  operationId: searchTwitter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scraperxpost\n  method: get\n  operationId: scrapeTwitterPost\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scraperxcomment\n  method: get\n  operationId: scrapeTwitterComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_run\n  method: post\n  operationId: runAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit\n  method: get\n  operationId: getAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_summary\n  method: get\n  operationId: getAuditSummary\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wavalidation\n  method: get\n  operationId: validateWhatsApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wavalidation\n  method: post\n  operationId: validateWhatsAppPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wavalidation/batch\n  method: post\n  operationId: submitWhatsAppBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /wavalidation/batch/{batch_id}\n  method: get\n  operationId: pollWhatsAppBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calleridvalidation\n  method: get\n  operationId: callerIdLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blacklistchecker\n  method: get\n  operationId: checkBlacklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spamchecker\n  method: post\n  operationId: checkSpam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /scrape\n  method: post\n  operationId: scrapeUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /google_serp\n  method: get\n  operationId: googleSerp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/proweblook-com/agentic-access/proweblook-com-agentic-access.yml
summary_line: 29 operations · 6 acting
tags:
- Verification
- Communications
- Security
- Data
---
