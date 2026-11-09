---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 63
api_specs:
- filename: prospectapis-pricing-api-openapi.yml
  format: yaml
  label: ProspectAPIs Pricing API
  slug: prospectapis-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-pricing-api-openapi.yml
- filename: prospectapis-watchlists-api-openapi.yml
  format: yaml
  label: ProspectAPIs Watchlists API
  slug: prospectapis-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-watchlists-api-openapi.yml
- filename: prospectapis-account-api-openapi.yml
  format: yaml
  label: ProspectAPIs Account API
  slug: prospectapis-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-account-api-openapi.yml
- filename: prospectapis-account-insights-api-openapi.yml
  format: yaml
  label: ProspectAPIs Account insights API
  slug: prospectapis-account-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-account-insights-api-openapi.yml
- filename: prospectapis-ads-api-openapi.yml
  format: yaml
  label: ProspectAPIs Ads API
  slug: prospectapis-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-ads-api-openapi.yml
- filename: prospectapis-companies-api-openapi.yml
  format: yaml
  label: ProspectAPIs Companies API
  slug: prospectapis-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-companies-api-openapi.yml
- filename: prospectapis-connected-account-api-openapi.yml
  format: yaml
  label: ProspectAPIs Connected account API
  slug: prospectapis-connected-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-connected-account-api-openapi.yml
- filename: prospectapis-email-verification-api-openapi.yml
  format: yaml
  label: ProspectAPIs Email verification API
  slug: prospectapis-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-email-verification-api-openapi.yml
- filename: prospectapis-events-api-openapi.yml
  format: yaml
  label: ProspectAPIs Events API
  slug: prospectapis-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-events-api-openapi.yml
- filename: prospectapis-funding-api-openapi.yml
  format: yaml
  label: ProspectAPIs Funding API
  slug: prospectapis-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-funding-api-openapi.yml
- filename: prospectapis-health-api-openapi.yml
  format: yaml
  label: ProspectAPIs Health API
  slug: prospectapis-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-health-api-openapi.yml
- filename: prospectapis-launches-api-openapi.yml
  format: yaml
  label: ProspectAPIs Launches API
  slug: prospectapis-launches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-launches-api-openapi.yml
- filename: prospectapis-messaging-reads-api-openapi.yml
  format: yaml
  label: ProspectAPIs Messaging reads API
  slug: prospectapis-messaging-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-messaging-reads-api-openapi.yml
- filename: prospectapis-meta-api-openapi.yml
  format: yaml
  label: ProspectAPIs Meta API
  slug: prospectapis-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-meta-api-openapi.yml
- filename: prospectapis-people-reads-api-openapi.yml
  format: yaml
  label: ProspectAPIs People reads API
  slug: prospectapis-people-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-people-reads-api-openapi.yml
- filename: prospectapis-people-writes-api-openapi.yml
  format: yaml
  label: ProspectAPIs People writes API
  slug: prospectapis-people-writes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-people-writes-api-openapi.yml
- filename: prospectapis-prospectapis-api-api-openapi.yml
  format: yaml
  label: ProspectAPIs ProspectAPIs API
  slug: prospectapis-prospectapis-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-prospectapis-api-api-openapi.yml
- filename: prospectapis-research-api-openapi.yml
  format: yaml
  label: ProspectAPIs Research API
  slug: prospectapis-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-research-api-openapi.yml
consequence_counts:
  physical: 5
  read: 63
  safety-critical: 3
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Prospectapis Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/accounts/connect-link/{link_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/email/verify/jobs/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/people/endorse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/people/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/people/invite/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/watchlists/{id}/test
operation_count: 107
overview: 'ProspectAPIs exposes 107 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 63 read, 36 write, 5 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ProspectAPIs
provider_slug: prospectapis
slug: prospectapis-agentic-access
source_filename: prospectapis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/prospectapis-health-api-openapi.yml, openapi/prospectapis-openapi.yml, openapi/prospectapis-pricing-api-openapi.yml,\n  openapi/prospectapis-prospectapis-api-api-openapi.yml, openapi/prospectapis-watchlists-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 107\n  by_action_class:\n    connected: 63\n    acting: 44\n  by_consequence:\n    read: 63\n    write: 36\n    safety-critical: 3\n    physical: 5\n  human_in_the_loop_required: 3\noperations:\n- path: /health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funding\n\
  \  method: get\n  operationId: searchFunding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funding/{id}\n  method: get\n  operationId: getFunding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research\n  method: post\n  operationId: submitResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/{id}\n  method: get\n  operationId: getResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/verify\n  method:\
  \ post\n  operationId: verifyEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/verify/stats\n  method: get\n  operationId: emailVerifyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/outcomes\n  method: post\n  operationId: reportEmailOutcomes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/find\n  method: post\n  operationId: emailFind\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/domain/{domain}\n  method: get\n  operationId: emailDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/verify/calibration\n  method: get\n  operationId: emailVerifyCalibration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/clean\n  method: post\n  operationId: emailClean\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/verify/jobs\n  method: post\n  operationId: createEmailVerifyJob\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/verify/jobs/{id}\n  method: get\n  operationId: getEmailVerifyJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/verify/jobs/{id}/results\n  method: get\n  operationId: getEmailVerifyJobResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/verify/jobs/{id}/stop\n  method: post\n  operationId: emailVerifyJobStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/watchlists\n  method: post\n  operationId: createWatchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists\n  method: get\n  operationId: listWatchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists/{id}\n  method: get\n  operationId: getWatchlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists/{id}\n  method: delete\n  operationId:\
  \ deleteWatchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{id}/test\n  method: post\n  operationId: testWatchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{id}/deliveries\n  method: get\n  operationId: listWatchlistDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId:\
  \ getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: sendFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: get\n  operationId: listFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback/{id}\n  method: get\n  operationId: getFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/version\n\
  \  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/profile\n  method: get\n  operationId: getPeopleProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/search\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/people/posts\n  method: get\n  operationId: getPeoplePosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/engagers\n  method: get\n  operationId: getPostEngagers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/resharers\n  method: get\n  operationId: getPostResharers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pages/followers\n  method: get\n  operationId: getPageFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pages/followers/enriched\n  method: get\n  operationId: getPageFollowersEnriched\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pages/profile\n  method: get\n  operationId: getPageProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/detail\n  method: get\n  operationId: getPostDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pages/search\n  method: post\n  operationId: searchPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/posts/search\n  method: post\n  operationId: searchPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/pages/employees\n  method: get\n  operationId: getPageEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads/search\n  method: post\n  operationId: searchLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/leads/companies/search\n  method: post\n  operationId: searchLeadCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{domain}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{domain}/funding\n  method: get\n  operationId: getCompanyFunding\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{domain}/jobs\n  method: get\n  operationId: getCompanyJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{domain}/technologies\n  method: get\n  operationId: getCompanyTechnologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/session\n  method: get\n  operationId: getAccountSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/session\n  method: post\n  operationId: connectAccountSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/session\n  method: delete\n  operationId: disconnectAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/login\n  method: post\n  operationId: connectAccountLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/inmail-credits\n  method: get\n  operationId: getMessageCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/react\n  method: post\n  operationId: reactToMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/read\n  method: post\n  operationId: markThreadRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chats\n  method: post\n  operationId: startChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/thread\n  method: get\n  operationId: readMessageThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invitations/received\n  method: get\n  operationId: listReceivedInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invitations/sent\n  method: get\n  operationId: listSentInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invitations/accept\n  method: post\n  operationId: acceptInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invitations/decline\n  method: post\n  operationId: declineInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/remove\n  method: post\n  operationId: removeConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/invite\n  method: post\n  operationId: invitePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/invite/withdraw\n  method: post\n  operationId: withdrawInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/follow\n  method: post\n  operationId: followPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/visit\n  method: post\n  operationId:\
  \ visitProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts\n  method: post\n  operationId: createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/react\n  method: post\n  operationId: reactToPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/comment\n\
  \  method: post\n  operationId: commentOnPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/repost\n  method: post\n  operationId: repostPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/quote\n  method: post\n  operationId: quotePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/launches\n  method: get\n  operationId: searchLaunches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/launches/{id}\n  method: get\n  operationId: getLaunch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ads\n  method: get\n  operationId: searchAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ads/{id}\n  method: get\n  operationId: getAd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/writes/queued\n  method: get\n  operationId: listQueuedWrites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/writes/queued/{id}\n  method: delete\n  operationId: cancelQueuedWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: get\n  operationId: listConnectedAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: post\n  operationId: addConnectedAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/accounts/{account_id}\n  method: get\n  operationId: getConnectedAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}\n  method: delete\n  operationId: removeConnectedAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/reconnect\n  method: post\n  operationId: reconnectConnectedAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/checkpoint\n\
  \  method: post\n  operationId: checkpointConnectedAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/edit\n  method: post\n  operationId: editPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/posts/delete\n  method: post\n  operationId: deletePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/posts/comment/delete\n  method: post\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/endorse\n  method: post\n  operationId: endorseSkill\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/people/skills\n  method: get\n  operationId: readPersonSkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/profile-views\n\
  \  method: get\n  operationId: readProfileViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/ssi\n  method: get\n  operationId: readSocialSellingIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/posts\n  method: get\n  operationId: readPostInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/connect-link\n  method: post\n  operationId: createAccountConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/accounts/connect-link/{link_id}\n  method: delete\n  operationId: revokeAccountConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/website/contacts\n  method: post\n  operationId: websiteContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: searchEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/cities\n  method: get\n  operationId: listEventCities\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/enrich\n  method: post\n  operationId: enrichEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricing\n  method: get\n  operationId: get_pricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{v1id}\n  method: get\n  operationId: get_v1_v1id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{v1id}\n  method: post\n  operationId: post_v1_v1id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{v1id}/{id}\n  method: get\n  operationId: get_v1_v1id_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists/{id}\n  method: delete\n  operationId: delete_v1_watchlists_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{id}/deliveries\n\
  \  method: get\n  operationId: get_v1_watchlists_id_deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists/{id}/test\n  method: post\n  operationId: post_v1_watchlists_id_test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/prospectapis/agentic-access/prospectapis-agentic-access.yml
summary_line: 107 operations · 44 acting · 3 human-in-the-loop
tags:
- Company
- Funding
- Research
- Data
- Funding Data
- Prospect Research
- Email Verification
- LinkedIn data
- Watchlist
- MCP
---
