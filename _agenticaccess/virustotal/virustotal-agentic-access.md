---
acting_count: 56
action_class_counts:
  acting: 56
  connected: 150
api_specs:
- filename: virustotal-access-control-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Access Control
  slug: virustotal-api-v3-access-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-access-control-openapi.yml
- filename: virustotal-ioc-feeds-openapi.yml
  format: yaml
  label: VirusTotal API v3 - IoC Feeds
  slug: virustotal-api-v3-ioc-feeds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-ioc-feeds-openapi.yml
- filename: virustotal-ioc-investigation-openapi.yml
  format: yaml
  label: VirusTotal API v3 - IoC Investigation
  slug: virustotal-api-v3-ioc-investigation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-ioc-investigation-openapi.yml
- filename: virustotal-private-scanning-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Private Scanning
  slug: virustotal-api-v3-private-scanning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-private-scanning-openapi.yml
- filename: virustotal-threat-graphs-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Threat Graphs
  slug: virustotal-api-v3-threat-graphs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-threat-graphs-openapi.yml
- filename: virustotal-threat-landscape-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Threat Landscape & Vulnerability Intelligence
  slug: virustotal-api-v3-threat-landscape-vulnerability-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-threat-landscape-openapi.yml
- filename: virustotal-yara-hunting-openapi.yml
  format: yaml
  label: VirusTotal API v3 - YARA Hunting (Livehunt, Retrohunt, IoC Stream)
  slug: virustotal-api-v3-yara-hunting-livehunt-retrohunt-ioc-stream
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-yara-hunting-openapi.yml
consequence_counts:
  physical: 6
  read: 150
  safety-critical: 11
  write: 39
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Virustotal Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /graphs/{id}/relationships/editors/{user_or_group_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /graphs/{id}/relationships/viewers/{user_or_group_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /groups/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /groups/{id}/relationships/administrators
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /groups/{id}/relationships/administrators/{user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /groups/{id}/relationships/service_accounts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /groups/{id}/relationships/users
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /groups/{id}/relationships/users/{user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /intelligence/hunting_rulesets/{id}/relationships/editors/{user_or_group_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /users/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /collections/{id}/{relationship}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collections/{id}/{relationship}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /graphs/{id}/relationships/editors
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /graphs/{id}/relationships/viewers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intelligence/hunting_rulesets/{id}/relationships/editors
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intelligence/hunting_rulesets/{id}/relationships/owner
operation_count: 206
overview: 'VirusTotal exposes 206 API operations that an AI agent could call, of which 56 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 150 read, 39 write, 6 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VirusTotal
provider_slug: virustotal
slug: virustotal-agentic-access
source_filename: virustotal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/virustotal-access-control-openapi.yml, openapi/virustotal-ioc-feeds-openapi.yml,\n  openapi/virustotal-ioc-investigation-openapi.yml, openapi/virustotal-private-scanning-openapi.yml,\n  openapi/virustotal-threat-graphs-openapi.yml, openapi/virustotal-threat-landscape-openapi.yml,\n  openapi/virustotal-yara-hunting-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 206\n  by_action_class:\n    connected: 150\n    acting: 56\n  by_consequence:\n    read: 150\n    safety-critical: 11\n    write: 39\n    physical: 6\n  human_in_the_loop_required: 11\noperations:\n- path: /groups/{id}\n  method: get\n  operationId: groups\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}\n  method: patch\n  operationId: patchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{id}/relationships/administrators\n  method: get\n  operationId: getGroupAdministrators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/relationships/administrators\n  method: post\n  operationId: postGroupAdministrators\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n  \
  \    purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{id}/relationships/administrators/{user_id}\n  method: delete\n  operationId: deleteUserGroupAdministrator\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{id}/relationships/administrators/{user_id}\n  method: get\n  operationId: checkUserGroupAdministrator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/relationships/users\n  method: get\n  operationId: getGroupUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/relationships/users\n  method: post\n  operationId: updateGroupUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{id}/relationships/users/{user_id}\n  method: delete\n  operationId: deleteUserFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{id}/relationships/users/{user_id}\n  method: get\n  operationId: checkUserInGroup\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/relationships/{relationship}\n  method: get\n  operationId: groupsRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/{relationship}\n  method: get\n  operationId: groupsRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/api_usage\n  method: get\n  operationId: userApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/overall_quotas\n  method: get\n  operationId: getUserOverallQuotas\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/api_usage\n  method: get\n  operationId: groupApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/relationships/service_accounts\n  method: get\n  operationId: getServiceAccountsOfAGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{id}/relationships/service_accounts\n  method: post\n  operationId: createANewServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /service_accounts/{id}\n\
  \  method: get\n  operationId: getAServiceAccountObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: delete\n  operationId: deleteUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: patch\n  operationId: patchUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/{id}/relationships/{relationship}\n  method: get\n  operationId: getUsersRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/{relationship}\n  method: get\n  operationId: usersRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/domains/hourly/{time}\n  method: get\n  operationId: feedsdomainshourly2time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/domains/{time}\n  method: get\n  operationId: feedsdomains2time\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/files/hourly/{time}\n  method: get\n  operationId: feedsFileHourly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/files/{time}\n  method: get\n  operationId: feedsFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/files/{token}/download\n  method: get\n  operationId: fileFeedDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ip_addresses/hourly/{time}\n  method: get\n  operationId: feedsipAddresseshourly2time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /feeds/ip_addresses/{time}\n  method: get\n  operationId: feedsipAddressestime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/file_behaviours/hourly/{time}\n  method: get\n  operationId: feedsFileBehaviourHourly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/file_behaviours/{time}\n  method: get\n  operationId: feedsFileBehaviour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/file_behaviours/{token}/evtx\n  method: get\n  operationId: fileBehaviourFeedEvtx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /feeds/file_behaviours/{token}/html\n  method: get\n  operationId: fileBehaviourFeedHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/file_behaviours/{token}/memdump\n  method: get\n  operationId: fileBehaviourFeedMemdump\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/file_behaviours/{token}/pcap\n  method: get\n  operationId: fileBehaviourFeedPcap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/urls/hourly/{time}\n  method: get\n  operationId: feedsUrlHourly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/urls/{time}\n  method:\
  \ get\n  operationId: feedsUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyses/{id}\n  method: get\n  operationId: analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyses/{id}/relationships/{relationship}\n  method: get\n  operationId: analysesGetDescriptors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyses/{id}/{relationship}\n  method: get\n  operationId: analysesGetObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{id}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/{id}\n  method: get\n  operationId: getOperationsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack_tactics/{id}\n  method: get\n  operationId: attackTacticsid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack_tactics/{id}/relationships/{relationship}\n  method: get\n  operationId: attackTacticsidrelationshipsrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack_tactics/{id}/{relationship}\n  method: get\n  operationId: attackTacticsidrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack_techniques/{id}\n  method: get\n  operationId: attackTechniqueid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack_techniques/{id}/relationships/{relationship}\n  method: get\n  operationId: attackTechniquesidrelationshipsrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack_techniques/{id}/{relationship}\n  method: get\n  operationId: attackTechniqueidrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /comments/{id}\n  method: delete\n  operationId: commentIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments/{id}/relationships/{relationship}\n  method: get\n  operationId: commentsRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments/{id}/vote\n  method: post\n  operationId: voteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments/{id}/{relationship}\n  method: get\n  operationId: commentsRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}\n  method: get\n  operationId: domainInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/comments\n  method: get\n  operationId: domainsCommentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/comments\n  method: post\n  operationId: domainsCommentsPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{domain}/relationships/{relationship}\n  method: get\n  operationId: domainsRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/votes\n  method: get\n  operationId: domainsVotesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/votes\n  method: post\n  operationId: domainVotesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{domain}/{relationship}\n  method: get\n  operationId: domainsRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resolutions/{id}\n  method: get\n  operationId: getResolutionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/upload_url\n  method: get\n  operationId: filesUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: filesScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{id}\n  method: get\n  operationId: fileInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/analyse\n  method: post\n  operationId: filesAnalyse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{id}/comments\n  method: get\n  operationId: filesCommentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/comments\n  method: post\n  operationId: filesCommentsPost\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{id}/download\n  method: get\n  operationId: filesDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/download_url\n  method: get\n  operationId: filesDownloadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/relationships/{relationship}\n  method: get\n  operationId: filesRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/votes\n  method: get\n  operationId: filesVotesGet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/votes\n  method: post\n  operationId: filesVotesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{id}/{relationship}\n  method: get\n  operationId: filesRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sigma_rules/{id}\n  method: get\n  operationId: getSigmaRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yara_rulesets/{id}\n  method: get\n  operationId:\
  \ getYaraRulesets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}\n  method: get\n  operationId: getFileBehaviourId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}/evtx\n  method: get\n  operationId: fileBehaviourEvtx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}/html\n  method: get\n  operationId: getFileBehaviourHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}/memdump\n  method: get\n  operationId: fileBehaviourMemdump\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}/pcap\n  method: get\n  operationId: fileBehavioursPcap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}/relationships/{relationship}\n  method: get\n  operationId: fileBehaviourssandboxIdrelationshipsrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_behaviours/{sandbox_id}/{relationship}\n  method: get\n  operationId: fileBehaviourssandboxIdrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/behaviour_mitre_trees\n  method: get\n  operationId:\
  \ getASummaryOfAllMitreAttckTechniquesObservedInAFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/behaviour_summary\n  method: get\n  operationId: fileAllBehavioursSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/behaviours\n  method: get\n  operationId: getAllBehaviorReportsForAFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip_addresses/{ip}\n  method: get\n  operationId: ipInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip_addresses/{ip}/comments\n  method: get\n  operationId: ipCommentsGet\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip_addresses/{ip}/comments\n  method: post\n  operationId: ipCommentsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_addresses/{ip}/relationships/{relationship}\n  method: get\n  operationId: ipRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip_addresses/{ip}/votes\n  method: get\n  operationId: ipVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip_addresses/{ip}/votes\n  method:\
  \ post\n  operationId: ipVotesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip_addresses/{ip}/{relationship}\n  method: get\n  operationId: ipRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /popular_threat_categories\n  method: get\n  operationId: popularThreatCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intelligence/search\n  method: get\n  operationId: intelligenceSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /intelligence/search/snippets/{snippet}\n  method: get\n  operationId: intelligenceSearchSnippets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: apiSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /urls\n  method: post\n  operationId: scanUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /urls/{id}\n  method: get\n  operationId: urlInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /urls/{id}/analyse\n  method: post\n  operationId: urlsAnalyse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /urls/{id}/comments\n  method: get\n  operationId: urlsCommentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /urls/{id}/comments\n  method: post\n  operationId: urlsCommentsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /urls/{id}/relationships/{relationship}\n  method: get\n  operationId: urlsRelationshipsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /urls/{id}/votes\n  method: get\n  operationId: urlsVotesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /urls/{id}/votes\n  method: post\n  operationId: urlsVotesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /urls/{id}/{relationship}\n  method: get\n  operationId:\
  \ urlsRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intelligence/zip_files\n  method: post\n  operationId: zipFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intelligence/zip_files/{id}\n  method: get\n  operationId: getZipFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intelligence/zip_files/{id}/download\n  method: get\n  operationId: zipFilesDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intelligence/zip_files/{id}/download_url\n\
  \  method: get\n  operationId: zipFilesDownloadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/analyses\n  method: get\n  operationId: listPrivateAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/analyses/{id}\n  method: get\n  operationId: privateAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/analyses/{id}/relationships/{relationship}\n  method: get\n  operationId: analysesidrelationshipsrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/analyses/{id}/{relationship}\n  method: get\n  operationId: analysesidrelationship\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/files\n  method: post\n  operationId: uploadFilePrivateScanning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private/files\n  method: get\n  operationId: listPrivateFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/files/upload_url\n  method: get\n  operationId: privateFilesUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/files/{id}\n  method: delete\n\
  \  operationId: deleteFilePrivateScanning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private/files/{id}\n  method: get\n  operationId: privateFilesInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/files/{id}/relationships/{relationship}\n  method: get\n  operationId: privatefilesidrelationshipsrelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/files/{id}/{relationship}\n  method: get\n  operationId: privateFilesRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/files/{sha256}/analyse\n  method: post\n  operationId: rescanAPrivateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private/file/{id}/behaviours\n  method: get\n  operationId: getAllBehaviourReportsFromAPrivateFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/file_behaviours/{sandbox_id}\n  method: get\n  operationId: privatefileBehaviourssandboxId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private/file_behaviours/{sandbox_id}/evtx\n  method:\
  \ get\n  operationId: fileBehaviourssandboxIdevtx\n  x-agentic-access:\n    action-class: conne\n\n# --- truncated at 32 KB (54 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/agentic-access/virustotal-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/agentic-access/virustotal-agentic-access.yml
summary_line: 206 operations · 56 acting · 11 human-in-the-loop
tags:
- Anti-Malware
- Threat Intelligence
- Security
- File Analysis
- URL Analysis
- YARA
- IoC
- Sandbox
- MITRE ATT&CK
- Google Cloud
---
